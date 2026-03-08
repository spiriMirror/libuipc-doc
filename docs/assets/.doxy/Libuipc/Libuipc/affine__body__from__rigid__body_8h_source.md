

# File affine\_body\_from\_rigid\_body.h

[**File List**](files.md) **>** [**affine\_body**](dir_0434b40e061af98901db13a48821d02b.md) **>** [**affine\_body\_from\_rigid\_body.h**](affine__body__from__rigid__body_8h.md)

[Go to the documentation of this file](affine__body__from__rigid__body_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/common/dllexport.h>

namespace uipc::geometry::affine_body
{
UIPC_GEOMETRY_API Matrix12x12 from_rigid_body(
    Float            mass,
    const Vector3&   center_of_mass,
    const Matrix3x3& inertia_cm);

UIPC_GEOMETRY_API Matrix12x12 build_abd_mass_matrix(
    Float             m,
    const Vector3&    m_x_bar,
    const Matrix3x3&  m_x_bar_x_bar);
}  // namespace uipc::geometry::affine_body
```


