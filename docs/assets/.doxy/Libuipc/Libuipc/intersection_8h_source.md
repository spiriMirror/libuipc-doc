

# File intersection.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**intersection.h**](intersection_8h.md)

[Go to the documentation of this file](intersection_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/type_define.h>

namespace uipc::geometry
{
UIPC_GEOMETRY_API bool tri_edge_intersect(const Vector3& T0,
                                          const Vector3& T1,
                                          const Vector3& T2,
                                          const Vector3& E0,
                                          const Vector3& E1,
                                          bool&          coplanar,
                                          Vector3&       uvw_in_tri,
                                          Vector2&       uv_in_edge);

UIPC_GEOMETRY_API bool is_point_in_tet(const Vector3& T0,
                                       const Vector3& T1,
                                       const Vector3& T2,
                                       const Vector3& T3,
                                       const Vector3& P,
                                       Vector4& tuvw_in_tet  // the barycentric coordinates of the intersection point in the tet
);
}  // namespace uipc::geometry
```


