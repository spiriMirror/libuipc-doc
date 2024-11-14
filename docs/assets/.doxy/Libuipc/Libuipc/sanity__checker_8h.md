

# File sanity\_checker.h



[**FileList**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**sanity\_check**](dir_bc94a01fec317e710a764ca285cf9c79.md) **>** [**sanity\_checker.h**](sanity__checker_8h.md)

[Go to the source code of this file](sanity__checker_8h_source.md)



* `#include <uipc/common/macro.h>`
* `#include <uipc/sanity_check/i_sanity_checker.h>`
* `#include <uipc/sanity_check/sanity_checker_auto_register.h>`
* `#include <uipc/core/scene.h>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**uipc**](namespaceuipc.md) <br> |
| namespace | [**backend**](namespaceuipc_1_1backend.md) <br> |
| namespace | [**core**](namespaceuipc_1_1core.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**SanityChecker**](classuipc_1_1core_1_1_sanity_checker.md) <br> |

















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**REGISTER\_SANITY\_CHECKER**](sanity__checker_8h.md#define-register_sanity_checker) (SanityChecker) <br> |

## Macro Definition Documentation





### define REGISTER\_SANITY\_CHECKER 

```C++
#define REGISTER_SANITY_CHECKER (
    SanityChecker
) namespace auto_register                                                                          \
    {                                                                                                \
        static ::uipc::core::SanityCheckerAutoRegister UIPC_NAME_WITH_ID(SanityCheckerAutoRegister){ \
            ::uipc::core::detail::register_sanity_checker_creator<SanityChecker>()};                 \
    }
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/sanity_check/sanity_checker.h`

