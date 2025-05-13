

# Class uipc::geometry::AttributeSlot

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)



_Template class to represent a geometries attribute slot of type T in a geometries attribute collection._ [More...](#detailed-description)

* `#include <attribute_slot.h>`



Inherits the following classes: [uipc::geometry::IAttributeSlot](classuipc_1_1geometry_1_1_i_attribute_slot.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef T | [**value\_type**](#typedef-value_type)  <br> |








































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AttributeSlot**](#function-attributeslot) (std::string\_view m\_name, S&lt; [**Attribute**](classuipc_1_1geometry_1_1_attribute.md)&lt; T &gt; &gt; attribute, bool allow\_destroy) <br> |
|  span&lt; const T &gt; | [**view**](#function-view-22) () noexcept const<br>_Get the const attribute values._  |


## Public Functions inherited from uipc::geometry::IAttributeSlot

See [uipc::geometry::IAttributeSlot](classuipc_1_1geometry_1_1_i_attribute_slot.md)

| Type | Name |
| ---: | :--- |
|   | [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-iattributeslot-13) () = default<br> |
|   | [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-iattributeslot-23) (const [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &) = delete<br> |
|   | [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-iattributeslot-33) ([**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &&) noexcept<br> |
|  bool | [**allow\_destroy**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-allow_destroy) () noexcept const<br>_Check if the underlying attribute is allowed to be destroyed._  |
|  bool | [**is\_shared**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-is_shared) () noexcept const<br>_Check if the underlying attribute is shared._  |
|  std::string\_view | [**name**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-name) () noexcept const<br>_Get the name of the attribute slot._  |
|  [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) & | [**operator=**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-operator) (const [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &) = delete<br> |
|  [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) & | [**operator=**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-operator_1) ([**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &&) noexcept<br> |
|  SizeT | [**size**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-size) () noexcept const<br> |
|  Json | [**to\_json**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-to_json-12) (SizeT i) const<br> |
|  Json | [**to\_json**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-to_json-22) () const<br> |
|  std::string\_view | [**type\_name**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-type_name) () noexcept const<br>_Get the type name of data stored in the attribute slot._  |
| virtual  | [**~IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-iattributeslot) () = default<br> |














































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**do\_clone**](#function-do_clone) (std::string\_view name, bool allow\_destroy) override const<br> |
| virtual S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**do\_clone\_empty**](#function-do_clone_empty) (std::string\_view name, bool allow\_destroy) override const<br> |
| virtual void | [**do\_make\_owned**](#function-do_make_owned) () override<br> |
| virtual Json | [**do\_to\_json**](#function-do_to_json) (SizeT i) override const<br> |
| virtual bool | [**get\_allow\_destroy**](#function-get_allow_destroy) () noexcept override const<br> |
| virtual [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**get\_attribute**](#function-get_attribute-12) () noexcept override<br> |
| virtual const [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**get\_attribute**](#function-get_attribute-22) () noexcept override const<br> |
| virtual std::string\_view | [**get\_name**](#function-get_name) () noexcept override const<br> |
| virtual SizeT | [**get\_use\_count**](#function-get_use_count) () noexcept override const<br> |


## Protected Functions inherited from uipc::geometry::IAttributeSlot

See [uipc::geometry::IAttributeSlot](classuipc_1_1geometry_1_1_i_attribute_slot.md)

| Type | Name |
| ---: | :--- |
| virtual [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**attribute**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-attribute-12) () noexcept<br> |
| virtual const [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**attribute**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-attribute-22) () noexcept const<br> |
| virtual S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**clone**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-clone) (std::string\_view name, bool allow\_destroy) const<br> |
| virtual S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**clone\_empty**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-clone_empty) (std::string\_view name, bool allow\_destroy) const<br> |
| virtual S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**do\_clone**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_clone) (std::string\_view name, bool allow\_destroy) const = 0<br> |
| virtual S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**do\_clone\_empty**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_clone_empty) (std::string\_view name, bool allow\_destroy) const = 0<br> |
| virtual void | [**do\_make\_owned**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_make_owned) () = 0<br> |
| virtual Json | [**do\_to\_json**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_to_json) (SizeT i) const = 0<br> |
| virtual bool | [**get\_allow\_destroy**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_allow_destroy) () noexcept const = 0<br> |
| virtual [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**get\_attribute**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_attribute-12) () noexcept = 0<br> |
| virtual const [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**get\_attribute**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_attribute-22) () noexcept const = 0<br> |
| virtual std::string\_view | [**get\_name**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_name) () noexcept const = 0<br> |
| virtual SizeT | [**get\_use\_count**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_use_count) () const = 0<br> |
|  void | [**make\_owned**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-make_owned) () <br> |
|  SizeT | [**use\_count**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-use_count) () const<br> |






# Detailed Description




**Template parameters:**


* `T` The type of the attribute values. 




    
## Public Types Documentation




### typedef value\_type 

```C++
using uipc::geometry::AttributeSlot< T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function AttributeSlot 

```C++
uipc::geometry::AttributeSlot::AttributeSlot (
    std::string_view m_name,
    S< Attribute < T > > attribute,
    bool allow_destroy
) 
```




<hr>



### function view [2/2]

_Get the const attribute values._ 
```C++
span< const T > uipc::geometry::AttributeSlot::view () noexcept const
```





**Returns:**

`span<const T>` 





        

<hr>
## Protected Functions Documentation




### function do\_clone 

```C++
virtual S< IAttributeSlot > uipc::geometry::AttributeSlot::do_clone (
    std::string_view name,
    bool allow_destroy
) override const
```



Implements [*uipc::geometry::IAttributeSlot::do\_clone*](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_clone)


<hr>



### function do\_clone\_empty 

```C++
virtual S< IAttributeSlot > uipc::geometry::AttributeSlot::do_clone_empty (
    std::string_view name,
    bool allow_destroy
) override const
```



Implements [*uipc::geometry::IAttributeSlot::do\_clone\_empty*](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_clone_empty)


<hr>



### function do\_make\_owned 

```C++
virtual void uipc::geometry::AttributeSlot::do_make_owned () override
```



Implements [*uipc::geometry::IAttributeSlot::do\_make\_owned*](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_make_owned)


<hr>



### function do\_to\_json 

```C++
virtual Json uipc::geometry::AttributeSlot::do_to_json (
    SizeT i
) override const
```



Implements [*uipc::geometry::IAttributeSlot::do\_to\_json*](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_to_json)


<hr>



### function get\_allow\_destroy 

```C++
virtual bool uipc::geometry::AttributeSlot::get_allow_destroy () noexcept override const
```



Implements [*uipc::geometry::IAttributeSlot::get\_allow\_destroy*](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_allow_destroy)


<hr>



### function get\_attribute [1/2]

```C++
virtual IAttribute & uipc::geometry::AttributeSlot::get_attribute () noexcept override
```



Implements [*uipc::geometry::IAttributeSlot::get\_attribute*](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_attribute-12)


<hr>



### function get\_attribute [2/2]

```C++
virtual const IAttribute & uipc::geometry::AttributeSlot::get_attribute () noexcept override const
```



Implements [*uipc::geometry::IAttributeSlot::get\_attribute*](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_attribute-22)


<hr>



### function get\_name 

```C++
virtual std::string_view uipc::geometry::AttributeSlot::get_name () noexcept override const
```



Implements [*uipc::geometry::IAttributeSlot::get\_name*](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_name)


<hr>



### function get\_use\_count 

```C++
virtual SizeT uipc::geometry::AttributeSlot::get_use_count () noexcept override const
```



Implements [*uipc::geometry::IAttributeSlot::get\_use\_count*](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_use_count)


<hr>## Friends Documentation





### friend view [1/2]

_Get the non-const attribute values._ 
```C++
template<typename U>
span< U > uipc::geometry::AttributeSlot::view (
    AttributeSlot < U > & slot
) 
```





**Returns:**

`span<T>` 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/attribute_slot.h`

