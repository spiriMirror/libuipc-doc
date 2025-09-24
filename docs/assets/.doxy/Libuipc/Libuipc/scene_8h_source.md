

# File scene.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**scene.h**](scene_8h.md)

[Go to the documentation of this file](scene_8h.md)


```C++
#pragma once
#include <uipc/core/contact_tabular.h>
#include <uipc/core/subscene_tabular.h>
#include <uipc/core/constitution_tabular.h>
#include <uipc/core/object.h>
#include <uipc/core/object_collection.h>
#include <uipc/core/animator.h>
#include <uipc/core/diff_sim.h>
#include <uipc/core/sanity_checker.h>
#include <uipc/geometry/attribute_collection.h>

namespace uipc::core::internal
{
class Scene;
class World;
}  // namespace uipc::core::internal

namespace uipc::backend
{
class SceneVisitor;
class WorldVisitor;
}  // namespace uipc::backend

namespace uipc::sanity_check
{
class SanityChecker;
}

namespace uipc::core
{
class SceneSnapshotCommit;
class SceneSnapshot;

class UIPC_CORE_API Scene final
{
    friend class backend::SceneVisitor;
    friend class World;
    friend class Object;
    friend class sanity_check::SanityChecker;
    friend class Animation;
    friend class SceneFactory;
    friend class SceneSnapshot;
    friend struct fmt::formatter<Scene>;

  public:
    template <bool IsConst>
    class ConfigAttributesT
    {
        friend struct fmt::formatter<ConfigAttributesT<IsConst>>;
        using AttributeCollection = geometry::AttributeCollection;
        template <typename T>
        using AttributeSlot = geometry::AttributeSlot<T>;
        using AttributeCopy = geometry::AttributeCopy;

        using AutoAttributeCollection =
            std::conditional_t<IsConst, const AttributeCollection, AttributeCollection>;

        template <bool _IsConst>
        friend class ConfigAttributesT;

        template <typename T>
        friend class geometry::AttributeFriend;

      public:
        ConfigAttributesT(AutoAttributeCollection& attributes)
            : m_attributes(attributes)
        {
        }

        template <bool OtherIsConst>
        ConfigAttributesT(const ConfigAttributesT<OtherIsConst>& o) noexcept
            requires(IsConst)
            : m_attributes(o.m_attributes)
        {
        }

        ConfigAttributesT(const ConfigAttributesT& o)            = default;
        ConfigAttributesT(ConfigAttributesT&& o)                 = default;
        ConfigAttributesT& operator=(const ConfigAttributesT& o) = default;
        ConfigAttributesT& operator=(ConfigAttributesT&& o)      = default;

        template <typename T>
        [[nodiscard]] auto find(std::string_view name)
        {
            return m_attributes.template find<T>(name);
        }

        template <typename T>
        decltype(auto) create(std::string_view name, const T& init_value = {})
        {
            return m_attributes.template create<T>(name, init_value);
        }

        template <typename T>
        decltype(auto) share(std::string_view name, const AttributeSlot<T>& slot)
            requires(!IsConst)
        {
            return m_attributes.template share<T>(name, slot);
        }

        void destroy(std::string_view name)
            requires(!IsConst)
        {
            m_attributes.destroy(name);
        }

        void copy_from(ConfigAttributesT<true> other,
                       const AttributeCopy&    copy          = {},
                       span<const string>      include_names = {},
                       span<const string>      exclude_names = {})
            requires(!IsConst)
        {
            m_attributes.copy_from(other.m_attributes, copy, include_names, exclude_names);
        }

        Json to_json() const { return m_attributes.to_json(); }

        void update_from(const geometry::AttributeCollectionCommit& commit)
            requires(!IsConst)
        {
            m_attributes.update_from(commit);
        }

        void build_from(const AttributeCollection& ac)
            requires(!IsConst)
        {
            m_attributes = ac;
        }

      private:
        AutoAttributeCollection& m_attributes;
        friend class SceneFactory;
    };

    using ConfigAttributes  = ConfigAttributesT<false>;
    using CConfigAttributes = ConfigAttributesT<true>;

    explicit Scene(const Json& config = default_config());
    // Allow create a core::Scene from a core::internal::Scene
    explicit Scene(S<internal::Scene> scene) noexcept;

    Scene(const Scene&) = delete;
    Scene(Scene&&)      = default;

    ~Scene();

    static Json default_config() noexcept;

    class UIPC_CORE_API Objects
    {
        friend class Scene;

      public:
        S<Object>         create(std::string_view name = "") &&;
        S<Object>         find(IndexT id) && noexcept;
        vector<S<Object>> find(std::string_view name) && noexcept;
        void              destroy(IndexT id) &&;
        SizeT             size() const noexcept;
        SizeT             created_count() const noexcept;

      private:
        Objects(internal::Scene& scene) noexcept;
        internal::Scene& m_scene;
    };

    class UIPC_CORE_API CObjects
    {
        friend class Scene;

      public:
        S<const Object>         find(IndexT id) && noexcept;
        vector<S<const Object>> find(std::string_view name) && noexcept;
        SizeT                   size() const noexcept;
        SizeT                   created_count() const noexcept;

      private:
        CObjects(const internal::Scene& scene) noexcept;
        const internal::Scene& m_scene;
    };

    class UIPC_CORE_API Geometries
    {
        friend class Scene;

      public:
        ObjectGeometrySlots<geometry::Geometry> find(IndexT id) && noexcept;

      private:
        Geometries(internal::Scene& scene) noexcept;
        internal::Scene& m_scene;
    };

    class UIPC_CORE_API CGeometries
    {
        friend class Scene;

      public:
        ObjectGeometrySlots<const geometry::Geometry> find(IndexT id) && noexcept;

      private:
        CGeometries(const internal::Scene& scene) noexcept;
        const internal::Scene& m_scene;
    };

    ConfigAttributes  config() noexcept;
    CConfigAttributes config() const noexcept;

    ContactTabular&       contact_tabular() noexcept;
    const ContactTabular& contact_tabular() const noexcept;

    SubsceneTabular&       subscene_tabular() noexcept;
    const SubsceneTabular& subscene_tabular() const noexcept;

    ConstitutionTabular&       constitution_tabular() noexcept;
    const ConstitutionTabular& constitution_tabular() const noexcept;

    Objects  objects() noexcept;
    CObjects objects() const noexcept;

    Geometries  geometries() noexcept;
    CGeometries geometries() const noexcept;

    Animator&       animator();
    const Animator& animator() const;

    DiffSim&       diff_sim();
    const DiffSim& diff_sim() const;

    SanityChecker&       sanity_checker();
    const SanityChecker& sanity_checker() const;

    void update_from(const SceneSnapshotCommit& snapshot);

  private:
    S<internal::Scene> m_internal;
};
}  // namespace uipc::core

namespace fmt
{
template <>
struct UIPC_CORE_API formatter<uipc::core::Scene> : formatter<string_view>
{
    appender format(const uipc::core::Scene& c, format_context& ctx) const;
};
}  // namespace fmt
```


