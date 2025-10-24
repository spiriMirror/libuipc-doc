

# File prim.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**usd**](dir_127bf4b01602b8d031b5fde8b608abd9.md) **>** [**prim.h**](prim_8h.md)

[Go to the documentation of this file](prim_8h.md)


```C++
#pragma once
#include <uipc/usd/dllexport.h>
#include <uipc/common/smart_pointer.h>
#include <uipc/geometry/geometry.h>

namespace uipc::usd
{
class UIPC_USD_API Prim
{
  public:
    S<geometry::Geometry> to_geometry();
    void                  from_geometry(geometry::Geometry& geo);

  private:
    class Impl;
    friend class Stage;
    explicit Prim(S<Impl> impl);
    S<Impl> m_impl;
};
}  // namespace uipc::usd
```


