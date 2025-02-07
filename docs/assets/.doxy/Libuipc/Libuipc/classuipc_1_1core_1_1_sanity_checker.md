

# Class uipc::core::SanityChecker



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SanityChecker**](classuipc_1_1core_1_1_sanity_checker.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SanityChecker**](#function-sanitychecker) ([**Scene**](classuipc_1_1core_1_1_scene.md) & scene) <br> |
|  SanityCheckResult | [**check**](#function-check) (std::string\_view workspace) <br> |
|  void | [**clear**](#function-clear) () <br> |
|  const unordered\_map&lt; U64, S&lt; [**SanityCheckMessage**](classuipc_1_1core_1_1_sanity_check_message.md) &gt; &gt; & | [**errors**](#function-errors) () const<br> |
|  const unordered\_map&lt; U64, S&lt; [**SanityCheckMessage**](classuipc_1_1core_1_1_sanity_check_message.md) &gt; &gt; & | [**infos**](#function-infos) () const<br> |
|  void | [**report**](#function-report) () <br> |
|  const unordered\_map&lt; U64, S&lt; [**SanityCheckMessage**](classuipc_1_1core_1_1_sanity_check_message.md) &gt; &gt; & | [**warns**](#function-warns) () const<br> |
|   | [**~SanityChecker**](#function-sanitychecker) () <br> |




























## Public Functions Documentation




### function SanityChecker 

```C++
uipc::core::SanityChecker::SanityChecker (
    Scene & scene
) 
```




<hr>



### function check 

```C++
SanityCheckResult uipc::core::SanityChecker::check (
    std::string_view workspace
) 
```




<hr>



### function clear 

```C++
void uipc::core::SanityChecker::clear () 
```




<hr>



### function errors 

```C++
const unordered_map< U64, S< SanityCheckMessage > > & uipc::core::SanityChecker::errors () const
```




<hr>



### function infos 

```C++
const unordered_map< U64, S< SanityCheckMessage > > & uipc::core::SanityChecker::infos () const
```




<hr>



### function report 

```C++
void uipc::core::SanityChecker::report () 
```




<hr>



### function warns 

```C++
const unordered_map< U64, S< SanityCheckMessage > > & uipc::core::SanityChecker::warns () const
```




<hr>



### function ~SanityChecker 

```C++
uipc::core::SanityChecker::~SanityChecker () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/sanity_checker.h`

