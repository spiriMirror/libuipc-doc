

# File factory.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**factory.h**](factory_8h.md)

[Go to the documentation of this file](factory_8h.md)


```C++
#pragma once
#include <uipc/common/span.h>
#include <uipc/geometry/simplicial_complex.h>
#include <uipc/geometry/implicit_geometry.h>

namespace uipc::geometry
{
UIPC_GEOMETRY_API [[nodiscard]] SimplicialComplex tetmesh(span<const Vector3> Vs,
                                                          span<const Vector4i> Ts);
UIPC_GEOMETRY_API [[nodiscard]] SimplicialComplex trimesh(span<const Vector3> Vs,
                                                          span<const Vector3i> Fs);
UIPC_GEOMETRY_API [[nodiscard]] SimplicialComplex linemesh(span<const Vector3> Vs,
                                                           span<const Vector2i> Es);
UIPC_GEOMETRY_API [[nodiscard]] SimplicialComplex pointcloud(span<const Vector3> Vs);


UIPC_GEOMETRY_API [[nodiscard]] ImplicitGeometry halfplane(
    const Vector3& P = Vector3::Zero(), const Vector3& N = Vector3::UnitY());

UIPC_GEOMETRY_API [[nodiscard]] ImplicitGeometry ground(Float height = 0.0,
                                                        const Vector3& N = Vector3::UnitY());
}  // namespace uipc::geometry
```


