

# File attribute\_name.h

[**File List**](files.md) **>** [**builtin**](dir_e46c520626162f9e42d80fd08f196511.md) **>** [**attribute\_name.h**](attribute__name_8h.md)

[Go to the documentation of this file](attribute__name_8h.md)


```C++
#pragma once
#include <string_view>

#define UIPC_BUILTIN_ATTRIBUTE(name) constexpr std::string_view name = #name

namespace uipc::builtin
{
#include <uipc/builtin/details/attribute_name.h>
}  // namespace uipc::builtin

#undef UIPC_BUILTIN_ATTRIBUTE
```


