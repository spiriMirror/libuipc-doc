

# Class uipc::geometry::IAttribute



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md)



_An abstract class to represent a geometries attribute._ 

* `#include <attribute.h>`





Inherited by the following classes: [uipc::geometry::Attribute](classuipc_1_1geometry_1_1_attribute.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**IAttribute**](#function-iattribute) () = default<br> |
|  void | [**from\_json**](#function-from_json) (const Json & j) noexcept<br> |
|  SizeT | [**size**](#function-size) () noexcept const<br>_Get the size of the attribute._  |
|  Json | [**to\_json**](#function-to_json-12) (SizeT i) noexcept const<br> |
|  Json | [**to\_json**](#function-to_json-22) () noexcept const<br> |
|  std::string\_view | [**type\_name**](#function-type_name) () noexcept const<br>_Get the type name of data stored in the attribute slot._  |
| virtual  | [**~IAttribute**](#function-iattribute) () = default<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_clear**](#function-do_clear) () = 0<br> |
| virtual S&lt; [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) &gt; | [**do\_clone**](#function-do_clone) () const = 0<br> |
| virtual S&lt; [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) &gt; | [**do\_clone\_empty**](#function-do_clone_empty) () const = 0<br> |
| virtual void | [**do\_copy\_from**](#function-do_copy_from) (const [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & other, const [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md) & copy) noexcept = 0<br> |
| virtual void | [**do\_from\_json**](#function-do_from_json) (const Json & j) noexcept = 0<br> |
| virtual void | [**do\_reorder**](#function-do_reorder) (span&lt; const SizeT &gt; O) noexcept = 0<br> |
| virtual void | [**do\_reserve**](#function-do_reserve) (SizeT N) = 0<br> |
| virtual void | [**do\_resize**](#function-do_resize) (SizeT N) = 0<br> |
| virtual Json | [**do\_to\_json**](#function-do_to_json-12) (SizeT i) noexcept const = 0<br> |
| virtual Json | [**do\_to\_json**](#function-do_to_json-22) () noexcept const = 0<br> |
| virtual SizeT | [**get\_size**](#function-get_size) () const = 0<br> |
| virtual std::string\_view | [**get\_type\_name**](#function-get_type_name) () noexcept const = 0<br> |




## Public Functions Documentation




### function IAttribute 

```C++
uipc::geometry::IAttribute::IAttribute () = default
```




<hr>



### function from\_json 

```C++
void uipc::geometry::IAttribute::from_json (
    const Json & j
) noexcept
```




<hr>



### function size 

```C++
SizeT uipc::geometry::IAttribute::size () noexcept const
```




<hr>



### function to\_json [1/2]

```C++
Json uipc::geometry::IAttribute::to_json (
    SizeT i
) noexcept const
```




<hr>



### function to\_json [2/2]

```C++
Json uipc::geometry::IAttribute::to_json () noexcept const
```




<hr>



### function type\_name 

```C++
std::string_view uipc::geometry::IAttribute::type_name () noexcept const
```




<hr>



### function ~IAttribute 

```C++
virtual uipc::geometry::IAttribute::~IAttribute () = default
```




<hr>
## Protected Functions Documentation




### function do\_clear 

```C++
virtual void uipc::geometry::IAttribute::do_clear () = 0
```




<hr>



### function do\_clone 

```C++
virtual S< IAttribute > uipc::geometry::IAttribute::do_clone () const = 0
```




<hr>



### function do\_clone\_empty 

```C++
virtual S< IAttribute > uipc::geometry::IAttribute::do_clone_empty () const = 0
```




<hr>



### function do\_copy\_from 

```C++
virtual void uipc::geometry::IAttribute::do_copy_from (
    const IAttribute & other,
    const AttributeCopy & copy
) noexcept = 0
```




<hr>



### function do\_from\_json 

```C++
virtual void uipc::geometry::IAttribute::do_from_json (
    const Json & j
) noexcept = 0
```




<hr>



### function do\_reorder 

```C++
virtual void uipc::geometry::IAttribute::do_reorder (
    span< const SizeT > O
) noexcept = 0
```




<hr>



### function do\_reserve 

```C++
virtual void uipc::geometry::IAttribute::do_reserve (
    SizeT N
) = 0
```




<hr>



### function do\_resize 

```C++
virtual void uipc::geometry::IAttribute::do_resize (
    SizeT N
) = 0
```




<hr>



### function do\_to\_json [1/2]

```C++
virtual Json uipc::geometry::IAttribute::do_to_json (
    SizeT i
) noexcept const = 0
```




<hr>



### function do\_to\_json [2/2]

```C++
virtual Json uipc::geometry::IAttribute::do_to_json () noexcept const = 0
```




<hr>



### function get\_size 

```C++
virtual SizeT uipc::geometry::IAttribute::get_size () const = 0
```




<hr>



### function get\_type\_name 

```C++
virtual std::string_view uipc::geometry::IAttribute::get_type_name () noexcept const = 0
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/attribute.h`

