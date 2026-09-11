

# File tetrahedralization.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**tetrahedralization.h**](tetrahedralization_8h.md)

[Go to the documentation of this file](tetrahedralization_8h.md)


```C++
// Copyright (C) 2026 spiriMirror
// SPDX-License-Identifier: Apache-2.0
#pragma once
#include <uipc/geometry/simplicial_complex.h>
#include <utility>

namespace uipc::geometry
{
UIPC_GEOMETRY_API Json tetrahedralization_default_config();

UIPC_GEOMETRY_API std::pair<SimplicialComplex, Json> tetrahedralize(
    const SimplicialComplex& surface,
    const Json&              config = tetrahedralization_default_config());
}  // namespace uipc::geometry
```


