

# File points\_from\_volume.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**vdb**](dir_25c4270e0507639fcebea9a8642b71ea.md) **>** [**points\_from\_volume.h**](vdb_2points__from__volume_8h.md)

[Go to the documentation of this file](vdb_2points__from__volume_8h.md)


```C++
#pragma once
#include <uipc/vdb/dllexport.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::vdb
{
UIPC_VDB_API geometry::SimplicialComplex points_from_volume(const geometry::SimplicialComplex& sc,
                                                            Float resolution);
}
```


