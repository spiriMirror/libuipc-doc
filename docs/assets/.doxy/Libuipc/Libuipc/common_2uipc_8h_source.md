

# File uipc.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**uipc.h**](common_2uipc_8h.md)

[Go to the documentation of this file](common_2uipc_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/json.h>

namespace uipc
{
UIPC_CORE_API void        init(const Json& config);
UIPC_CORE_API Json        default_config();
UIPC_CORE_API const Json& config();
}  // namespace uipc
```


