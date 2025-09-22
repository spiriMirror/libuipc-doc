

# File attribute\_debug\_info.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**attribute\_debug\_info.h**](attribute__debug__info_8h.md)

[Go to the documentation of this file](attribute__debug__info_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/type_define.h>
#include <uipc/common/json.h>

namespace uipc::geometry
{
class UIPC_CORE_API AttributeDebugInfo
{
  public:
    static std::string& thread_local_last_not_found_name();
    static Json&        thread_local_extras();
};
}  // namespace uipc::geometry
```


