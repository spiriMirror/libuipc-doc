

# File config.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**config.h**](config_8h.md)

[Go to the documentation of this file](config_8h.md)


```C++
#pragma once

namespace uipc
{
#if UIPC_RUNTIME_CHECK
constexpr bool RUNTIME_CHECK = true;
#else
constexpr bool RUNTIME_CHECK = false;
#endif
}  // namespace uipc
```


