

# File attribute\_name.h



[**FileList**](files.md) **>** [**builtin**](dir_e46c520626162f9e42d80fd08f196511.md) **>** [**details**](dir_4db2109fccbcdb4025718aaa828a1196.md) **>** [**attribute\_name.h**](details_2attribute__name_8h.md)

[Go to the source code of this file](details_2attribute__name_8h_source.md)

_This file records all the built-in attribute names in the libuipc specification._ [More...](#detailed-description)


































































# Detailed Description


Programmers can define their own UIPC\_BUILTIN\_ATTRIBUTE macro outside this file, and include this file to get the built-in attribute names.



```C++
#define UIPC_BUILTIN_ATTRIBUTE(name) constexpr std::string_view name = #name
#include <pyuipc/builtin/attribute_name.h>
#undef UIPC_BUILTIN_ATTRIBUTE
```





**Author:**

MuGdxy 




**Date:**

September 2024 





    

------------------------------
The documentation for this class was generated from the following file `include/uipc/builtin/details/attribute_name.h`

