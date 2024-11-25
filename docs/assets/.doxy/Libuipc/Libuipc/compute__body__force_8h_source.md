

# File compute\_body\_force.h

[**File List**](files.md) **>** [**affine\_body**](dir_0434b40e061af98901db13a48821d02b.md) **>** [**compute\_body\_force.h**](compute__body__force_8h.md)

[Go to the documentation of this file](compute__body__force_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/common/dllexport.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::geometry::affine_body
{
UIPC_GEOMETRY_API Vector12 compute_body_force(const SimplicialComplex& sc,
                                              const Vector3& body_force_density);
}  // namespace uipc::geometry::affine_body
```


