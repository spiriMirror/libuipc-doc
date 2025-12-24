

# Class uipc::core::ISanityCheckerCollection



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ISanityCheckerCollection**](classuipc_1_1core_1_1ISanityCheckerCollection.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**build**](#function-build) ([**core::internal::Scene**](classuipc_1_1core_1_1internal_1_1Scene.md) & s) = 0<br> |
| virtual SanityCheckResult | [**check**](#function-check) ([**SanityCheckMessageCollection**](classuipc_1_1core_1_1SanityCheckMessageCollection.md) & msg) const = 0<br> |
| virtual  | [**~ISanityCheckerCollection**](#function-isanitycheckercollection) () = default<br> |




























## Public Functions Documentation




### function build 

```C++
virtual void uipc::core::ISanityCheckerCollection::build (
    core::internal::Scene & s
) = 0
```




<hr>



### function check 

```C++
virtual SanityCheckResult uipc::core::ISanityCheckerCollection::check (
    SanityCheckMessageCollection & msg
) const = 0
```




<hr>



### function ~ISanityCheckerCollection 

```C++
virtual uipc::core::ISanityCheckerCollection::~ISanityCheckerCollection () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/i_sanity_checker.h`

