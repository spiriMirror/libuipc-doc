

# Class uipc::core::ISanityChecker



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ISanityChecker**](classuipc_1_1core_1_1_i_sanity_checker.md)










Inherited by the following classes: [uipc::core::SanityChecker](classuipc_1_1core_1_1_sanity_checker.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  SanityCheckResult | [**check**](#function-check) () noexcept<br> |
|  U64 | [**id**](#function-id) () noexcept const<br> |
| virtual  | [**~ISanityChecker**](#function-isanitychecker) () = default<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual SanityCheckResult | [**do\_check**](#function-do_check) () noexcept = 0<br> |
| virtual U64 | [**get\_id**](#function-get_id) () noexcept const = 0<br> |




## Public Functions Documentation




### function check 

```C++
SanityCheckResult uipc::core::ISanityChecker::check () noexcept
```




<hr>



### function id 

```C++
U64 uipc::core::ISanityChecker::id () noexcept const
```




<hr>



### function ~ISanityChecker 

```C++
virtual uipc::core::ISanityChecker::~ISanityChecker () = default
```




<hr>
## Protected Functions Documentation




### function do\_check 

```C++
virtual SanityCheckResult uipc::core::ISanityChecker::do_check () noexcept = 0
```




<hr>



### function get\_id 

```C++
virtual U64 uipc::core::ISanityChecker::get_id () noexcept const = 0
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/sanity_check/i_sanity_checker.h`

