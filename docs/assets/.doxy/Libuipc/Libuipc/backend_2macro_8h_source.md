

# File macro.h

[**File List**](files.md) **>** [**backend**](dir_53d62147b82bd29328805b2087bd1012.md) **>** [**macro.h**](backend_2macro_8h.md)

[Go to the documentation of this file](backend_2macro_8h.md)


```C++
#pragma once

#ifdef _MSC_VER
#ifdef UIPC_BACKEND_EXPORT_DLL
#define UIPC_BACKEND_API __declspec(dllexport)
#else
#define UIPC_BACKEND_API __declspec(dllimport)
#endif

#else
#define UIPC_BACKEND_API
#endif
```


