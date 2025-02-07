

# File distance.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**distance.h**](distance_8h.md)

[Go to the documentation of this file](distance_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/common/dllexport.h>

namespace uipc::geometry
{
Float UIPC_GEOMETRY_API halfplane_vertex_signed_distance(const Vector3& P,
                                                         const Vector3& N,
                                                         const Vector3& V,
                                                         Float V_thickness = 0.0);

Float UIPC_GEOMETRY_API point_point_squared_distance(const Vector3& P0, const Vector3& P1);

Float UIPC_GEOMETRY_API point_edge_squared_distance(const Vector3& P,
                                                    const Vector3& E0,
                                                    const Vector3& E1);

Float UIPC_GEOMETRY_API point_triangle_squared_distance(const Vector3& P,
                                                        const Vector3& T0,
                                                        const Vector3& T1,
                                                        const Vector3& T2);

Float UIPC_GEOMETRY_API edge_edge_squared_distance(const Vector3& Ea0,
                                                   const Vector3& Ea1,
                                                   const Vector3& Eb0,
                                                   const Vector3& Eb1);
}  // namespace uipc::geometry
```


