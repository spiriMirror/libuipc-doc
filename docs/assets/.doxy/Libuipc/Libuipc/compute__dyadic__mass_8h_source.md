

# File compute\_dyadic\_mass.h

[**File List**](files.md) **>** [**affine\_body**](dir_0434b40e061af98901db13a48821d02b.md) **>** [**compute\_dyadic\_mass.h**](compute__dyadic__mass_8h.md)

[Go to the documentation of this file](compute__dyadic__mass_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/common/dllexport.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::geometry::affine_body
{
UIPC_GEOMETRY_API void compute_dyadic_mass(const SimplicialComplex& sc,
                                           Float                    rho,
                                           //tex: $$ \sum \mathbf{m} $$
                                           Float& m,
                                           //tex: $$ \sum \mathbf{m} \bar{\mathbf{x}} $$
                                           Vector3& m_x_bar,
                                           //tex: $$ \sum \mathbf{m} \bar{\mathbf{x}} \cdot \bar{\mathbf{x}}^T$$
                                           Matrix3x3& m_x_bar_x_bar);

UIPC_GEOMETRY_API void compute_dyadic_mass(const SimplicialComplex& sc,
                                           Float                    rho,
                                           Float                    thickness,
                                           Float&                   m,
                                           Vector3&                 m_x_bar,
                                           Matrix3x3& m_x_bar_x_bar);
}  // namespace uipc::geometry::affine_body
```


