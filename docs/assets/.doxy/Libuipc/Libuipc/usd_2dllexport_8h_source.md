

# File dllexport.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**usd**](dir_127bf4b01602b8d031b5fde8b608abd9.md) **>** [**dllexport.h**](usd_2dllexport_8h.md)

[Go to the documentation of this file](usd_2dllexport_8h.md)


```C++
#pragma once

#ifdef _WIN32
#ifdef UIPC_USD_EXPORT_DLL
#define UIPC_USD_API __declspec(dllexport)
#else
#define UIPC_USD_API __declspec(dllimport)
#endif
#else
#define UIPC_USD_API
#endif
```


