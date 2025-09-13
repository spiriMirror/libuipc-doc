

# File backend\_name.h



[**FileList**](files.md) **>** [**builtin**](dir_e46c520626162f9e42d80fd08f196511.md) **>** [**details**](dir_4db2109fccbcdb4025718aaa828a1196.md) **>** [**backend\_name.h**](backend__name_8h.md)

[Go to the source code of this file](backend__name_8h_source.md)

_This file records all the built-in backend names in the libuipc specification._ [More...](#detailed-description)


































































# Detailed Description


Programmers can define their own UIPC\_BUILTIN\_BACKEND macro outside this file, and include this file to get the built-in backend names.



```C++
#define UIPC_BUILTIN_BACKEND(name) constexpr std::string_view name = #name
#include <pyuipc/builtin/backend_name.h>
#undef UIPC_BUILTIN_BACKEND
```





**Author:**

MuGdxy 




**Date:**

September 2024 





    

------------------------------
The documentation for this class was generated from the following file `include/uipc/builtin/details/backend_name.h`

