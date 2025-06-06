

# File geometry\_collection\_commit.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**geometry\_collection\_commit.h**](geometry__collection__commit_8h.md)

[Go to the documentation of this file](geometry__collection__commit_8h.md)


```C++
#pragma once
#include <uipc/geometry/geometry_collection.h>
#include <uipc/geometry/geometry_commit.h>

namespace uipc::geometry
{
class UIPC_CORE_API GeometryCollectionCommit
{
    friend class GeometryFactory;

    friend UIPC_CORE_API GeometryCollectionCommit operator-(const GeometryCollection& dst,
                                                            const GeometryCollection& src);
    friend UIPC_CORE_API GeometryCollection& operator+=(GeometryCollection& dst,
                                                        const GeometryCollectionCommit& inc);

  public:
    GeometryCollectionCommit() = default;

    GeometryCollectionCommit(const GeometryCollectionCommit&);
    GeometryCollectionCommit& operator=(const GeometryCollectionCommit&) = delete;

    GeometryCollectionCommit(const GeometryCollection& dst, const GeometryCollection& src);

  private:
    IndexT m_next_id = 0;

    unordered_map<IndexT, S<GeometryCommit>> m_geometries;
};

UIPC_CORE_API GeometryCollectionCommit operator-(const GeometryCollection& dst,
                                                 const GeometryCollection& src);
UIPC_CORE_API GeometryCollection&      operator+=(GeometryCollection& dst,
                                             const GeometryCollectionCommit& inc);

}  // namespace uipc::geometry
```


