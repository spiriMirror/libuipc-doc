

# File implicit\_geometry\_uid\_auto\_register.h



[**FileList**](files.md) **>** [**builtin**](dir_e46c520626162f9e42d80fd08f196511.md) **>** [**implicit\_geometry\_uid\_auto\_register.h**](implicit__geometry__uid__auto__register_8h.md)

[Go to the source code of this file](implicit__geometry__uid__auto__register_8h_source.md)



* `#include <uipc/builtin/uid_register.h>`
* `#include <uipc/common/list.h>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**uipc**](namespaceuipc.md) <br> |
| namespace | [**builtin**](namespaceuipc_1_1builtin.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**ImplicitGeometryUIDAutoRegister**](classuipc_1_1builtin_1_1_implicit_geometry_u_i_d_auto_register.md) <br> |

















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**REGISTER\_IMPLICIT\_GEOMETRY\_UIDS**](implicit__geometry__uid__auto__register_8h.md#define-register_implicit_geometry_uids) (...) `REGISTER\_IMPLICIT\_GEOMETRY\_UIDS\_INTERNAL(\_\_COUNTER\_\_)`<br>_Register ImplicitGeometryUIDs._  |
| define  | [**REGISTER\_IMPLICIT\_GEOMETRY\_UIDS\_INTERNAL**](implicit__geometry__uid__auto__register_8h.md#define-register_implicit_geometry_uids_internal) (counter) `/* multi line expression */`<br> |

## Macro Definition Documentation





### define REGISTER\_IMPLICIT\_GEOMETRY\_UIDS 

_Register ImplicitGeometryUIDs._ 
```C++
#define REGISTER_IMPLICIT_GEOMETRY_UIDS (
    ...
) `REGISTER_IMPLICIT_GEOMETRY_UIDS_INTERNAL(__COUNTER__)`
```



Example:



```C++
REGISTER_IMPLICIT_GEOMETRY_UIDS()
{
    using namespace uipc::builtin;
    list<UIDInfo> uids;
    return uids;
}
```
 


        

<hr>



### define REGISTER\_IMPLICIT\_GEOMETRY\_UIDS\_INTERNAL 

```C++
#define REGISTER_IMPLICIT_GEOMETRY_UIDS_INTERNAL (
    counter
) `/* multi line expression */`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/builtin/implicit_geometry_uid_auto_register.h`

