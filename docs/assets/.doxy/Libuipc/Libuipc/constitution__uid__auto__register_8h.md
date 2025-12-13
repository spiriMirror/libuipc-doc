

# File constitution\_uid\_auto\_register.h



[**FileList**](files.md) **>** [**builtin**](dir_e46c520626162f9e42d80fd08f196511.md) **>** [**constitution\_uid\_auto\_register.h**](constitution__uid__auto__register_8h.md)

[Go to the source code of this file](constitution__uid__auto__register_8h_source.md)



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
| class | [**ConstitutionUIDAutoRegister**](classuipc_1_1builtin_1_1_constitution_u_i_d_auto_register.md) <br> |

















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**REGISTER\_CONSTITUTION\_UIDS**](constitution__uid__auto__register_8h.md#define-register_constitution_uids) (...) `REGISTER\_CONSTITUTION\_UIDS\_INTERNAL(\_\_COUNTER\_\_)`<br>_Register ConstitutionUIDs._  |
| define  | [**REGISTER\_CONSTITUTION\_UIDS\_INTERNAL**](constitution__uid__auto__register_8h.md#define-register_constitution_uids_internal) (counter) `/* multi line expression */`<br> |

## Macro Definition Documentation





### define REGISTER\_CONSTITUTION\_UIDS 

_Register ConstitutionUIDs._ 
```C++
#define REGISTER_CONSTITUTION_UIDS (
    ...
) `REGISTER_CONSTITUTION_UIDS_INTERNAL(__COUNTER__)`
```



Example:



```C++
REGISTER_CONSTITUTION_UIDS()
{
    using namespace uipc::builtin;
    list<UIDInfo> uids;
    return uids;
}
```
 


        

<hr>



### define REGISTER\_CONSTITUTION\_UIDS\_INTERNAL 

```C++
#define REGISTER_CONSTITUTION_UIDS_INTERNAL (
    counter
) `/* multi line expression */`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/builtin/constitution_uid_auto_register.h`

