

# File attribute\_collection.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**attribute\_collection.h**](attribute__collection_8h.md)

[Go to the documentation of this file](attribute__collection_8h.md)


```C++
#pragma once
#include <uipc/common/string.h>
#include <uipc/common/unordered_map.h>
#include <uipc/common/exception.h>
#include <uipc/common/smart_pointer.h>
#include <uipc/geometry/attribute.h>
#include <uipc/geometry/attribute_slot.h>
#include <uipc/geometry/attribute_copy.h>

namespace uipc::geometry
{
class UIPC_CORE_API AttributeCollection
{
    friend struct fmt::formatter<AttributeCollection>;

  public:
    AttributeCollection() = default;

    AttributeCollection(const AttributeCollection&);
    AttributeCollection& operator=(const AttributeCollection&);

    AttributeCollection(AttributeCollection&&) noexcept;
    AttributeCollection& operator=(AttributeCollection&&) noexcept;

    template <typename T>
    S<AttributeSlot<T>> create(std::string_view name,
                               const T&         default_value = {},
                               bool             allow_destroy = true);

    S<IAttributeSlot> share(std::string_view      name,
                            const IAttributeSlot& slot,
                            bool                  allow_destroy = true);

    template <typename T>
    S<AttributeSlot<T>> share(std::string_view        name,
                              const AttributeSlot<T>& slot,
                              bool                    allow_destroy = true);

    void destroy(std::string_view name);

    [[nodiscard]] S<IAttributeSlot> find(std::string_view name);
    [[nodiscard]] S<const IAttributeSlot> find(std::string_view name) const;

    template <typename T>
    [[nodiscard]] S<AttributeSlot<T>> find(std::string_view name);

    template <typename T>
    [[nodiscard]] S<const AttributeSlot<T>> find(std::string_view name) const;

    void resize(SizeT N);

    void reorder(span<const SizeT> O);

    void copy_from(const AttributeCollection& other,
                   const AttributeCopy&       copy,
                   span<const string>         include_names = {},
                   span<const string>         exclude_names = {});

    [[nodiscard]] SizeT size() const;
    void clear();
    void reserve(SizeT N);

    vector<string> names() const;

    SizeT attribute_count() const;

    Json to_json() const;

  private:
    SizeT                                    m_size = 0;
    unordered_map<string, S<IAttributeSlot>> m_attributes;
};

class UIPC_CORE_API GeometryAttributeError : public Exception
{
  public:
    using Exception::Exception;
};
}  // namespace uipc::geometry


namespace fmt
{
template <>
struct UIPC_CORE_API formatter<uipc::geometry::AttributeCollection>
    : formatter<std::string_view>
{
    appender format(const uipc::geometry::AttributeCollection& collection,
                    format_context&                            ctx) const;
};
}  // namespace fmt


#include "details/attribute_collection.inl"
```


