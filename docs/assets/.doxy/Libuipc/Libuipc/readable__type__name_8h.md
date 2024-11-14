

# File readable\_type\_name.h



[**FileList**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**readable\_type\_name.h**](readable__type__name_8h.md)

[Go to the source code of this file](readable__type__name_8h_source.md)



* `#include <uipc/common/type_define.h>`
* `#include <string_view>`
* `#include <boost/core/demangle.hpp>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**uipc**](namespaceuipc.md) <br> |



















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](readable__type__name_8h.md#define-readable_type_name_as_alias) (type) <br> |

## Macro Definition Documentation





### define READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
#define READABLE_TYPE_NAME_AS_ALIAS (
    type
) template <>                                                                \
    inline std::string readable_type_name<type>() noexcept                     \
    {                                                                          \
        return #type;                                                          \
    }
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/readable_type_name.h`

