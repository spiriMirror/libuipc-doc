

# File demangle.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**demangle.h**](demangle_8h.md)

[Go to the documentation of this file](demangle_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <typeinfo>
#include <string>

namespace uipc
{
UIPC_CORE_API std::string demangle(const std::string& mangled_name);

template <typename T>
inline std::string demangle() noexcept
{
    return demangle(typeid(T).name());
}
}  // namespace uipc
```


