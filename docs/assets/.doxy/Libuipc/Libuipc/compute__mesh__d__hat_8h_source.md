

# File compute\_mesh\_d\_hat.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**compute\_mesh\_d\_hat.h**](compute__mesh__d__hat_8h.md)

[Go to the documentation of this file](compute__mesh__d__hat_8h.md)


```C++
#pragma once
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::geometry
{
UIPC_GEOMETRY_API S<AttributeSlot<Float>> compute_mesh_d_hat(
    SimplicialComplex& R, Float max_d_hat = std::numeric_limits<Float>::max());
}  // namespace uipc::geometry
```


