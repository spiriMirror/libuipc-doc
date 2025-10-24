

# File stage.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**usd**](dir_127bf4b01602b8d031b5fde8b608abd9.md) **>** [**stage.h**](stage_8h.md)

[Go to the documentation of this file](stage_8h.md)


```C++
#pragma once
#include <uipc/usd/prim.h>

namespace uipc::usd
{
class UIPC_USD_API Stage
{
  public:
    static Stage open(std::string_view path);
    Prim         get_prim_at_path(std::string_view path) const;
    ~Stage();
  private:
    class Impl;
    explicit Stage(S<Impl> impl);
    S<Impl> m_impl;
};
}  // namespace uipc::usd
```


