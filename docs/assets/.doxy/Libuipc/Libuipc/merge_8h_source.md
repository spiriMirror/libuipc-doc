

# File merge.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**merge.h**](merge_8h.md)

[Go to the documentation of this file](merge_8h.md)


```C++
#pragma once
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::geometry
{
UIPC_GEOMETRY_API [[nodiscard]] SimplicialComplex merge(span<const SimplicialComplex*> complexes);

UIPC_GEOMETRY_API [[nodiscard]] SimplicialComplex merge(span<const SimplicialComplex> complexes);

UIPC_GEOMETRY_API [[nodiscard]] SimplicialComplex merge(
    std::initializer_list<const SimplicialComplex*>&& complexes);
}  // namespace uipc::geometry
```


