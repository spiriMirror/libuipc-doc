

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

    IndexT create(const Geometry& geo, bool evolving_only = false);

    S<const GeometrySlot> find(IndexT id) const;

    SizeT geometry_count() const noexcept;

    void create(std::string_view name, const AttributeCollection& ac, bool evolving_only = false);

    S<const AttributeCollection> find(std::string_view name) const;

    SizeT attribute_collection_count() const noexcept;

    vector<std::string> attribute_collection_names() const noexcept;

    Json to_json() const;

    void from_json(const Json& j);

  private:
    U<Impl> m_impl;
};

class UIPC_CORE_API GeometryAtlasCommit
{
    class Impl;

  public:
    GeometryAtlasCommit();
    ~GeometryAtlasCommit();

    IndexT                  create(const GeometryCommit& geo_commit);
    S<const GeometryCommit> find(IndexT id) const;
    void create(std::string_view name, const AttributeCollectionCommit& ac_commit);
    S<const AttributeCollectionCommit> find(std::string_view name) const;
    vector<std::string> attribute_collection_names() const noexcept;
    SizeT               attribute_collection_count() const noexcept;
    SizeT               geometry_count() const noexcept;

    Json to_json() const;

    void from_json(const Json& j);


    U<Impl> m_impl;
};
}  // namespace uipc::geometry
```


