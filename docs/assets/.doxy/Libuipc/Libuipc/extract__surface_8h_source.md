

# File extract\_surface.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**extract\_surface.h**](extract__surface_8h.md)

[Go to the documentation of this file](extract__surface_8h.md)


```C++
#pragma once
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::geometry
{
UIPC_GEOMETRY_API [[nodiscard]] SimplicialComplex extract_surface(const SimplicialComplex& src);

UIPC_GEOMETRY_API [[nodiscard]] SimplicialComplex extract_surface(span<const SimplicialComplex*> complexes);
}  // namespace uipc::geometry
```


