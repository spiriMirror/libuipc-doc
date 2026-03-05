

# File closest\_vertex\_edge\_pairs.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**closest\_vertex\_edge\_pairs.h**](closest__vertex__edge__pairs_8h.md)

[Go to the documentation of this file](closest__vertex__edge__pairs_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/common/dllexport.h>
#include <uipc/common/span.h>
#include <string_view>

namespace uipc::geometry
{
class SimplicialComplex;
class Geometry;

Geometry UIPC_GEOMETRY_API closest_vertex_edge_pairs(const SimplicialComplex& vertex_mesh,
                                                     const SimplicialComplex& edge_mesh,
                                                     Float max_distance);
}  // namespace uipc::geometry
```


