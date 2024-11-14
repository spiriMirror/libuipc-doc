

# File log\_pattern\_guard.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**log\_pattern\_guard.h**](log__pattern__guard_8h.md)

[Go to the documentation of this file](log__pattern__guard_8h.md)


```C++
#pragma once
#include <spdlog/spdlog.h>
#include <uipc/common/dllexport.h>
namespace uipc
{
class UIPC_CORE_API LogPatternGuard
{
  public:
    LogPatternGuard(std::string_view pattern) noexcept;
    ~LogPatternGuard() noexcept;
};
}  // namespace uipc
```


