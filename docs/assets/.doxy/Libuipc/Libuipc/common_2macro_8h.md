

# File macro.h



[**FileList**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**macro.h**](common_2macro_8h.md)

[Go to the source code of this file](common_2macro_8h_source.md)



































































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**UIPC\_CONCATE**](common_2macro_8h.md#define-uipc_concate) (x, y) `x##y`<br> |
| define  | [**UIPC\_NAME\_WITH\_ID**](common_2macro_8h.md#define-uipc_name_with_id) (x) `UIPC\_NAME\_WITH\_ID\_IMPL(x, \_\_COUNTER\_\_)`<br> |
| define  | [**UIPC\_NAME\_WITH\_ID\_IMPL**](common_2macro_8h.md#define-uipc_name_with_id_impl) (x, ID) `UIPC\_CONCATE(x, ID)`<br> |
| define  | [**UIPC\_TO\_STRING**](common_2macro_8h.md#define-uipc_to_string) (x) `#x`<br> |

## Macro Definition Documentation





### define UIPC\_CONCATE 

```C++
#define UIPC_CONCATE (
    x,
    y
) `x##y`
```




<hr>



### define UIPC\_NAME\_WITH\_ID 

```C++
#define UIPC_NAME_WITH_ID (
    x
) `UIPC_NAME_WITH_ID_IMPL(x, __COUNTER__)`
```




<hr>



### define UIPC\_NAME\_WITH\_ID\_IMPL 

```C++
#define UIPC_NAME_WITH_ID_IMPL (
    x,
    ID
) `UIPC_CONCATE(x, ID)`
```




<hr>



### define UIPC\_TO\_STRING 

```C++
#define UIPC_TO_STRING (
    x
) `#x`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/macro.h`

