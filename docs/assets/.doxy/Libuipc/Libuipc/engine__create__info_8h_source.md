

# File engine\_create\_info.h

[**File List**](files.md) **>** [**backend**](dir_53d62147b82bd29328805b2087bd1012.md) **>** [**engine\_create\_info.h**](engine__create__info_8h.md)

[Go to the documentation of this file](engine__create__info_8h.md)


```C++
#pragma once
#include <string_view>

namespace uipc::backend
{
class EngineCreateInfo
{
  public:
    std::string_view workspace;
};
}  // namespace uipc::backend

using EngineCreateInfo = uipc::backend::EngineCreateInfo;
```


