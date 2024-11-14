

# File compute\_vertex\_mass.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**compute\_vertex\_mass.h**](compute__vertex__mass_8h.md)

[Go to the documentation of this file](compute__vertex__mass_8h.md)


```C++
#pragma once
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::geometry
{
UIPC_GEOMETRY_API S<AttributeSlot<Float>> compute_vertex_mass(SimplicialComplex& R,
                                                              Float mass_density);
}  // namespace uipc::geometry
```


