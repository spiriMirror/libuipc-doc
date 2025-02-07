

# File optimal\_transform.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**optimal\_transform.h**](optimal__transform_8h.md)

[Go to the documentation of this file](optimal__transform_8h.md)


```C++
#pragma once
#include "uipc/common/dllexport.h"
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::geometry
{
UIPC_GEOMETRY_API Matrix4x4 optimal_transform(span<const Vector3> S, span<const Vector3> D);

UIPC_GEOMETRY_API Matrix4x4 optimal_transform(const SimplicialComplex& S, const SimplicialComplex& D);
}  // namespace uipc::geometry
```


