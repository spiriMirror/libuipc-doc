

# File module\_info.h

[**File List**](files.md) **>** [**backend**](dir_53d62147b82bd29328805b2087bd1012.md) **>** [**module\_info.h**](module__info_8h.md)

[Go to the documentation of this file](module__info_8h.md)


```C++
#pragma once
#include <cstdint>

inline constexpr std::uint32_t UIPC_BACKEND_ABI_VERSION = 1;

struct UIPCBackendModuleInfo
{
    std::uint32_t struct_size;
    std::uint32_t abi_version;
    std::uint32_t uipc_version_major;
    std::uint32_t uipc_version_minor;
    std::uint32_t uipc_version_patch;
    const char*   backend_name;
};
```


