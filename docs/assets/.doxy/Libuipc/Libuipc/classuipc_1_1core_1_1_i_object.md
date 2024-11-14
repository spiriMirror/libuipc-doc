

# Class uipc::core::IObject



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**IObject**](classuipc_1_1core_1_1_i_object.md)










Inherited by the following classes: [uipc::core::Object](classuipc_1_1core_1_1_object.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  IndexT | [**id**](#function-id) () noexcept const<br> |
|  std::string\_view | [**name**](#function-name) () noexcept const<br> |
| virtual  | [**~IObject**](#function-iobject) () = default<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual IndexT | [**get\_id**](#function-get_id) () noexcept const = 0<br> |
| virtual std::string\_view | [**get\_name**](#function-get_name) () noexcept const = 0<br> |




## Public Functions Documentation




### function id 

```C++
IndexT uipc::core::IObject::id () noexcept const
```




<hr>



### function name 

```C++
std::string_view uipc::core::IObject::name () noexcept const
```




<hr>



### function ~IObject 

```C++
virtual uipc::core::IObject::~IObject () = default
```




<hr>
## Protected Functions Documentation




### function get\_id 

```C++
virtual IndexT uipc::core::IObject::get_id () noexcept const = 0
```




<hr>



### function get\_name 

```C++
virtual std::string_view uipc::core::IObject::get_name () noexcept const = 0
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/object.h`

