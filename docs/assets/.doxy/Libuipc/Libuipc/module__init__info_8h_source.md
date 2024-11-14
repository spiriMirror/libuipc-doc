

# File module\_init\_info.h

[**File List**](files.md) **>** [**backend**](dir_53d62147b82bd29328805b2087bd1012.md) **>** [**module\_init\_info.h**](module__init__info_8h.md)

[Go to the documentation of this file](module__init__info_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <memory_resource>


class UIPC_CORE_API UIPCModuleInitInfo
{
  public:
    std::string_view           module_name;
    std::pmr::memory_resource* memory_resource = nullptr;
};
```


