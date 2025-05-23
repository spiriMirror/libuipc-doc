

# File scene\_snapshot.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**scene\_snapshot.h**](scene__snapshot_8h.md)

[Go to the documentation of this file](scene__snapshot_8h.md)


```C++
#pragma once
#include <uipc/core/scene.h>
#include <uipc/geometry/geometry_commit.h>
#include <uipc/core/object_collection.h>

namespace uipc::core
{
class UIPC_CORE_API SceneSnapshot
{
    friend class Scene;
    friend class SceneSnapshotCommit;
    friend class SceneFactory;

  public:
    SceneSnapshot(const Scene& scene);
    SceneSnapshot(const SceneSnapshot&)            = default;
    SceneSnapshot(SceneSnapshot&&)                 = default;
    SceneSnapshot& operator=(const SceneSnapshot&) = default;
    SceneSnapshot& operator=(SceneSnapshot&&)      = default;

  private:
    SceneSnapshot() = default;
    Json                     m_config;
    ObjectCollectionSnapshot m_object_collection;
    vector<ContactElement>   m_contact_elements;


    unordered_map<IndexT, S<geometry::Geometry>> m_geometries;
    unordered_map<IndexT, S<geometry::Geometry>> m_rest_geometries;

    geometry::AttributeCollection m_contact_models;
};

class UIPC_CORE_API SceneSnapshotCommit
{
    friend class SceneFactory;
    friend SceneSnapshotCommit UIPC_CORE_API operator-(const SceneSnapshot& dst,
                                                       const SceneSnapshot& src);
    friend class internal::Scene;

  public:
    SceneSnapshotCommit() = default;
    SceneSnapshotCommit(const SceneSnapshot& dst, const SceneSnapshot& src);

    bool        is_valid() const noexcept { return m_is_valid; }
    const Json& config() const noexcept { return m_config; }
    const ObjectCollectionSnapshot& object_collection() const noexcept
    {
        return m_object_collection;
    }
    const vector<ContactElement>& contact_elements() const noexcept
    {
        return m_contact_elements;
    }

    const unordered_map<IndexT, geometry::GeometryCommit>& geometries() const noexcept
    {
        return m_geometries;
    }

    const unordered_map<IndexT, geometry::GeometryCommit>& rest_geometries() const noexcept
    {
        return m_rest_geometries;
    }

    const geometry::AttributeCollectionCommit& contact_models() const noexcept
    {
        return m_contact_models;
    }

  private:
    bool m_is_valid = true;
    // Fully Copy:
    Json                     m_config;
    ObjectCollectionSnapshot m_object_collection;
    vector<ContactElement>   m_contact_elements;

    // Full Copy Geometries/ Diff Copy AttributeCollection
    unordered_map<IndexT, geometry::GeometryCommit> m_geometries;
    unordered_map<IndexT, geometry::GeometryCommit> m_rest_geometries;

    // Diff Copy AttributeCollection
    geometry::AttributeCollectionCommit m_contact_models;
};

SceneSnapshotCommit UIPC_CORE_API operator-(const SceneSnapshot& dst,
                                            const SceneSnapshot& src);
}  // namespace uipc::core
```


