

# Class uipc::core::ISanityChecker



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ISanityChecker**](classuipc_1_1core_1_1_i_sanity_checker.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**build**](#function-build) () <br> |
|  SanityCheckResult | [**check**](#function-check) ([**SanityCheckMessage**](classuipc_1_1core_1_1_sanity_check_message.md) & msg) <br> |
|  U64 | [**id**](#function-id) () noexcept const<br> |
|  std::string | [**name**](#function-name) () noexcept const<br> |
| virtual  | [**~ISanityChecker**](#function-isanitychecker) () = default<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual SanityCheckResult | [**do\_check**](#function-do_check) ([**SanityCheckMessage**](classuipc_1_1core_1_1_sanity_check_message.md) & msg) = 0<br> |
| virtual U64 | [**get\_id**](#function-get_id) () noexcept const = 0<br> |
| virtual std::string | [**get\_name**](#function-get_name) () noexcept const = 0<br> |




## Public Functions Documentation




### function build 

```C++
virtual void uipc::core::ISanityChecker::build () 
```




<hr>



### function check 

```C++
SanityCheckResult uipc::core::ISanityChecker::check (
    SanityCheckMessage & msg
) 
```




<hr>



### function id 

```C++
U64 uipc::core::ISanityChecker::id () noexcept const
```




<hr>



### function name 

```C++
std::string uipc::core::ISanityChecker::name () noexcept const
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
virtual SanityCheckResult uipc::core::ISanityChecker::do_check (
    SanityCheckMessage & msg
) = 0
```




<hr>



### function get\_id 

```C++
virtual U64 uipc::core::ISanityChecker::get_id () noexcept const = 0
```




<hr>



### function get\_name 

```C++
virtual std::string uipc::core::ISanityChecker::get_name () noexcept const = 0
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/i_sanity_checker.h`

