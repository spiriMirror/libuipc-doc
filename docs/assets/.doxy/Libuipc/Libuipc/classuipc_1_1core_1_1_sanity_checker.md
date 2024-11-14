

# Class uipc::core::SanityChecker



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SanityChecker**](classuipc_1_1core_1_1_sanity_checker.md)








Inherits the following classes: [uipc::core::ISanityChecker](classuipc_1_1core_1_1_i_sanity_checker.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SanityChecker**](#function-sanitychecker) ([**Scene**](classuipc_1_1core_1_1_scene.md) & s) noexcept<br> |
| virtual SanityCheckResult | [**do\_check**](#function-do_check-12) () noexcept<br> |
| virtual U64 | [**get\_id**](#function-get_id) () noexcept const = 0<br> |


## Public Functions inherited from uipc::core::ISanityChecker

See [uipc::core::ISanityChecker](classuipc_1_1core_1_1_i_sanity_checker.md)

| Type | Name |
| ---: | :--- |
|  SanityCheckResult | [**check**](classuipc_1_1core_1_1_i_sanity_checker.md#function-check) () noexcept<br> |
|  U64 | [**id**](classuipc_1_1core_1_1_i_sanity_checker.md#function-id) () noexcept const<br> |
| virtual  | [**~ISanityChecker**](classuipc_1_1core_1_1_i_sanity_checker.md#function-isanitychecker) () = default<br> |














## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**Scene**](classuipc_1_1core_1_1_scene.md) & | [**m\_scene**](#variable-m_scene)  <br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual SanityCheckResult | [**do\_check**](#function-do_check-22) ([**backend::SceneVisitor**](classuipc_1_1backend_1_1_scene_visitor.md) & scene) noexcept = 0<br> |


## Protected Functions inherited from uipc::core::ISanityChecker

See [uipc::core::ISanityChecker](classuipc_1_1core_1_1_i_sanity_checker.md)

| Type | Name |
| ---: | :--- |
| virtual SanityCheckResult | [**do\_check**](classuipc_1_1core_1_1_i_sanity_checker.md#function-do_check) () noexcept = 0<br> |
| virtual U64 | [**get\_id**](classuipc_1_1core_1_1_i_sanity_checker.md#function-get_id) () noexcept const = 0<br> |






## Public Functions Documentation




### function SanityChecker 

```C++
explicit uipc::core::SanityChecker::SanityChecker (
    Scene & s
) noexcept
```




<hr>



### function do\_check [1/2]

```C++
virtual SanityCheckResult uipc::core::SanityChecker::do_check () noexcept
```



Implements [*uipc::core::ISanityChecker::do\_check*](classuipc_1_1core_1_1_i_sanity_checker.md#function-do_check)


<hr>



### function get\_id 

```C++
virtual U64 uipc::core::SanityChecker::get_id () noexcept const = 0
```



Implements [*uipc::core::ISanityChecker::get\_id*](classuipc_1_1core_1_1_i_sanity_checker.md#function-get_id)


<hr>
## Protected Attributes Documentation




### variable m\_scene 

```C++
Scene& uipc::core::SanityChecker::m_scene;
```




<hr>
## Protected Functions Documentation




### function do\_check [2/2]

```C++
virtual SanityCheckResult uipc::core::SanityChecker::do_check (
    backend::SceneVisitor & scene
) noexcept = 0
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/sanity_check/sanity_checker.h`

