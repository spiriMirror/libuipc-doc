

# File dllexport.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**vdb**](dir_25c4270e0507639fcebea9a8642b71ea.md) **>** [**dllexport.h**](vdb_2dllexport_8h.md)

[Go to the documentation of this file](vdb_2dllexport_8h.md)


```C++
#pragma once

#ifdef _WIN32
#ifdef UIPC_VDB_EXPORT_DLL
#define UIPC_VDB_API __declspec(dllexport)
#else
#define UIPC_VDB_API __declspec(dllimport)
#endif
#else
#define UIPC_VDB_API
#endif
```


