

# Class uipc::core::SanityCheckerAutoRegister



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SanityCheckerAutoRegister**](classuipc_1_1core_1_1_sanity_checker_auto_register.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**Creators**](classuipc_1_1core_1_1_sanity_checker_auto_register_1_1_creators.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::function&lt; U&lt; [**ISanityChecker**](classuipc_1_1core_1_1_i_sanity_checker.md) &gt;([**Scene**](classuipc_1_1core_1_1_scene.md) &)&gt; | [**Creator**](#typedef-creator)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SanityCheckerAutoRegister**](#function-sanitycheckerautoregister) (Creator && reg) <br> |




























## Public Types Documentation




### typedef Creator 

```C++
using uipc::core::SanityCheckerAutoRegister::Creator =  std::function<U<ISanityChecker>(Scene&)>;
```




<hr>
## Public Functions Documentation




### function SanityCheckerAutoRegister 

```C++
uipc::core::SanityCheckerAutoRegister::SanityCheckerAutoRegister (
    Creator && reg
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/sanity_check/sanity_checker_auto_register.h`

