

# Class uipc::geometry::Attribute

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**Attribute**](classuipc_1_1geometry_1_1_attribute.md)



_Template class to represent a geometries attribute of type T._ [More...](#detailed-description)

* `#include <attribute.h>`



Inherits the following classes: [uipc::geometry::IAttribute](classuipc_1_1geometry_1_1_i_attribute.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |








































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Attribute**](#function-attribute-13) (const T & default\_value={}) noexcept<br> |
|   | [**Attribute**](#function-attribute-23) (const [**Attribute**](classuipc_1_1geometry_1_1_attribute.md)&lt; T &gt; &) = default<br> |
|   | [**Attribute**](#function-attribute-33) ([**Attribute**](classuipc_1_1geometry_1_1_attribute.md)&lt; T &gt; &&) = default<br> |
|  [**Attribute**](classuipc_1_1geometry_1_1_attribute.md)&lt; T &gt; & | [**operator=**](#function-operator) (const [**Attribute**](classuipc_1_1geometry_1_1_attribute.md)&lt; T &gt; &) = default<br> |
|  [**Attribute**](classuipc_1_1geometry_1_1_attribute.md)&lt; T &gt; & | [**operator=**](#function-operator_1) ([**Attribute**](classuipc_1_1geometry_1_1_attribute.md)&lt; T &gt; &&) = default<br> |
|  span&lt; const T &gt; | [**view**](#function-view-22) () noexcept const<br> |


## Public Functions inherited from uipc::geometry::IAttribute

See [uipc::geometry::IAttribute](classuipc_1_1geometry_1_1_i_attribute.md)

| Type | Name |
| ---: | :--- |
|   | [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md#function-iattribute) () = default<br> |
|  SizeT | [**size**](classuipc_1_1geometry_1_1_i_attribute.md#function-size) () noexcept const<br>_Get the size of the attribute._  |
|  Json | [**to\_json**](classuipc_1_1geometry_1_1_i_attribute.md#function-to_json-12) (SizeT i) noexcept const<br> |
|  Json | [**to\_json**](classuipc_1_1geometry_1_1_i_attribute.md#function-to_json-22) () noexcept const<br> |
| virtual  | [**~IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md#function-iattribute) () = default<br> |














































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_clear**](#function-do_clear) () override<br> |
| virtual S&lt; [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) &gt; | [**do\_clone**](#function-do_clone) () override const<br> |
| virtual S&lt; [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) &gt; | [**do\_clone\_empty**](#function-do_clone_empty) () override const<br> |
| virtual void | [**do\_copy\_from**](#function-do_copy_from) (const [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & other, const [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md) & copy) noexcept override<br> |
| virtual void | [**do\_reorder**](#function-do_reorder) (span&lt; const SizeT &gt; O) noexcept override<br> |
| virtual void | [**do\_reserve**](#function-do_reserve) (SizeT N) override<br> |
| virtual void | [**do\_resize**](#function-do_resize) (SizeT N) override<br> |
| virtual Json | [**do\_to\_json**](#function-do_to_json) (SizeT i) noexcept override const<br> |
| virtual [**backend::BufferView**](classuipc_1_1backend_1_1_buffer_view.md) | [**get\_backend\_view**](#function-get_backend_view) () noexcept override const<br> |
| virtual SizeT | [**get\_size**](#function-get_size) () override const<br> |


## Protected Functions inherited from uipc::geometry::IAttribute

See [uipc::geometry::IAttribute](classuipc_1_1geometry_1_1_i_attribute.md)

| Type | Name |
| ---: | :--- |
|  [**backend::BufferView**](classuipc_1_1backend_1_1_buffer_view.md) | [**backend\_view**](classuipc_1_1geometry_1_1_i_attribute.md#function-backend_view-22) () noexcept const<br> |
| virtual void | [**do\_clear**](classuipc_1_1geometry_1_1_i_attribute.md#function-do_clear) () = 0<br> |
| virtual S&lt; [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) &gt; | [**do\_clone**](classuipc_1_1geometry_1_1_i_attribute.md#function-do_clone) () const = 0<br> |
| virtual S&lt; [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) &gt; | [**do\_clone\_empty**](classuipc_1_1geometry_1_1_i_attribute.md#function-do_clone_empty) () const = 0<br> |
| virtual void | [**do\_copy\_from**](classuipc_1_1geometry_1_1_i_attribute.md#function-do_copy_from) (const [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & other, const [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md) & copy) noexcept = 0<br> |
| virtual void | [**do\_reorder**](classuipc_1_1geometry_1_1_i_attribute.md#function-do_reorder) (span&lt; const SizeT &gt; O) noexcept = 0<br> |
| virtual void | [**do\_reserve**](classuipc_1_1geometry_1_1_i_attribute.md#function-do_reserve) (SizeT N) = 0<br> |
| virtual void | [**do\_resize**](classuipc_1_1geometry_1_1_i_attribute.md#function-do_resize) (SizeT N) = 0<br> |
| virtual Json | [**do\_to\_json**](classuipc_1_1geometry_1_1_i_attribute.md#function-do_to_json) (SizeT i) noexcept const = 0<br> |
| virtual [**backend::BufferView**](classuipc_1_1backend_1_1_buffer_view.md) | [**get\_backend\_view**](classuipc_1_1geometry_1_1_i_attribute.md#function-get_backend_view) () noexcept const = 0<br> |
| virtual SizeT | [**get\_size**](classuipc_1_1geometry_1_1_i_attribute.md#function-get_size) () const = 0<br> |






# Detailed Description




**Template parameters:**


* `T` The type of the attribute values. 




    
## Public Types Documentation




### typedef value\_type 

```C++
using uipc::geometry::Attribute< T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function Attribute [1/3]

```C++
uipc::geometry::Attribute::Attribute (
    const T & default_value={}
) noexcept
```




<hr>



### function Attribute [2/3]

```C++
uipc::geometry::Attribute::Attribute (
    const Attribute < T > &
) = default
```




<hr>



### function Attribute [3/3]

```C++
uipc::geometry::Attribute::Attribute (
    Attribute < T > &&
) = default
```




<hr>



### function operator= 

```C++
Attribute < T > & uipc::geometry::Attribute::operator= (
    const Attribute < T > &
) = default
```




<hr>



### function operator= 

```C++
Attribute < T > & uipc::geometry::Attribute::operator= (
    Attribute < T > &&
) = default
```




<hr>



### function view [2/2]

```C++
span< const T > uipc::geometry::Attribute::view () noexcept const
```




<hr>
## Protected Functions Documentation




### function do\_clear 

```C++
virtual void uipc::geometry::Attribute::do_clear () override
```



Implements [*uipc::geometry::IAttribute::do\_clear*](classuipc_1_1geometry_1_1_i_attribute.md#function-do_clear)


<hr>



### function do\_clone 

```C++
virtual S< IAttribute > uipc::geometry::Attribute::do_clone () override const
```



Implements [*uipc::geometry::IAttribute::do\_clone*](classuipc_1_1geometry_1_1_i_attribute.md#function-do_clone)


<hr>



### function do\_clone\_empty 

```C++
virtual S< IAttribute > uipc::geometry::Attribute::do_clone_empty () override const
```



Implements [*uipc::geometry::IAttribute::do\_clone\_empty*](classuipc_1_1geometry_1_1_i_attribute.md#function-do_clone_empty)


<hr>



### function do\_copy\_from 

```C++
virtual void uipc::geometry::Attribute::do_copy_from (
    const IAttribute & other,
    const AttributeCopy & copy
) noexcept override
```



Implements [*uipc::geometry::IAttribute::do\_copy\_from*](classuipc_1_1geometry_1_1_i_attribute.md#function-do_copy_from)


<hr>



### function do\_reorder 

```C++
virtual void uipc::geometry::Attribute::do_reorder (
    span< const SizeT > O
) noexcept override
```



Implements [*uipc::geometry::IAttribute::do\_reorder*](classuipc_1_1geometry_1_1_i_attribute.md#function-do_reorder)


<hr>



### function do\_reserve 

```C++
virtual void uipc::geometry::Attribute::do_reserve (
    SizeT N
) override
```



Implements [*uipc::geometry::IAttribute::do\_reserve*](classuipc_1_1geometry_1_1_i_attribute.md#function-do_reserve)


<hr>



### function do\_resize 

```C++
virtual void uipc::geometry::Attribute::do_resize (
    SizeT N
) override
```



Implements [*uipc::geometry::IAttribute::do\_resize*](classuipc_1_1geometry_1_1_i_attribute.md#function-do_resize)


<hr>



### function do\_to\_json 

```C++
virtual Json uipc::geometry::Attribute::do_to_json (
    SizeT i
) noexcept override const
```



Implements [*uipc::geometry::IAttribute::do\_to\_json*](classuipc_1_1geometry_1_1_i_attribute.md#function-do_to_json)


<hr>



### function get\_backend\_view 

```C++
virtual backend::BufferView uipc::geometry::Attribute::get_backend_view () noexcept override const
```



Implements [*uipc::geometry::IAttribute::get\_backend\_view*](classuipc_1_1geometry_1_1_i_attribute.md#function-get_backend_view)


<hr>



### function get\_size 

```C++
virtual SizeT uipc::geometry::Attribute::get_size () override const
```



Implements [*uipc::geometry::IAttribute::get\_size*](classuipc_1_1geometry_1_1_i_attribute.md#function-get_size)


<hr>## Friends Documentation





### friend view [1/2]

```C++
inline span< T > uipc::geometry::Attribute::view (
    Attribute < T > & a
) noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/attribute.h`

