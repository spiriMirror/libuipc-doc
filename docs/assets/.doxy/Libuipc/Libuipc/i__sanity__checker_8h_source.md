

# File i\_sanity\_checker.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**sanity\_check**](dir_bc94a01fec317e710a764ca285cf9c79.md) **>** [**i\_sanity\_checker.h**](i__sanity__checker_8h.md)

[Go to the documentation of this file](i__sanity__checker_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/type_define.h>

namespace uipc::core
{
class Scene;

enum class SanityCheckResult : int
{
    Success = 0,
    Warning = 1,
    Error   = 2
};

class UIPC_CORE_API ISanityChecker
{
  public:
    virtual ~ISanityChecker() = default;
    U64               id() const noexcept;
    SanityCheckResult check() noexcept;

  protected:
    virtual U64               get_id() const noexcept = 0;
    virtual SanityCheckResult do_check() noexcept     = 0;
};
}  // namespace uipc::core
```


