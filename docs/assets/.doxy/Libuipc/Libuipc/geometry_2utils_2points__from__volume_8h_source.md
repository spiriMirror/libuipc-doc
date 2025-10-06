

# File points\_from\_volume.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**points\_from\_volume.h**](geometry_2utils_2points__from__volume_8h.md)

[Go to the documentation of this file](geometry_2utils_2points__from__volume_8h.md)


```C++
#pragma once
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::geometry
{
UIPC_GEOMETRY_API SimplicialComplex points_from_volume(const SimplicialComplex& sc,
                                                       Float resolution = 0.01);
}  // namespace uipc::geometry
```


