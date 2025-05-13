

# File geometry\_atlas.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**geometry\_atlas.h**](geometry__atlas_8h.md)

[Go to the documentation of this file](geometry__atlas_8h.md)


```C++
#pragma once
#include <uipc/geometry/geometry.h>
#include <uipc/geometry/geometry_slot.h>
#include <uipc/geometry/geometry_collection.h>

namespace uipc::geometry
{
class UIPC_CORE_API GeometryAtlas
{
    class Impl;

  public:
    GeometryAtlas();
    ~GeometryAtlas();

    IndexT create(const Geometry& geo);

    const GeometrySlot* find(IndexT id) const;

    SizeT geometry_count() const noexcept;

    void create(std::string_view name, const AttributeCollection& ac);

    const AttributeCollection* find(std::string_view name) const;

    SizeT attribute_collection_count() const noexcept;

    vector<std::string> attribute_collection_names() const noexcept;

    Json to_json() const;

    void from_json(const Json& j);

  private:
    U<Impl> m_impl;
};
}  // namespace uipc::geometry
```


