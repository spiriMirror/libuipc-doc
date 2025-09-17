

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
|   | [**AttributeSlot**](#function-attributeslot-12) (std::string\_view name, S&lt; [**Attribute**](classuipc_1_1geometry_1_1_attribute.md)&lt; T &gt; &gt; attribute, bool allow\_destroy) <br> |
|   | [**AttributeSlot**](#function-attributeslot-22) (std::string\_view name, S&lt; [**Attribute**](classuipc_1_1geometry_1_1_attribute.md)&lt; T &gt; &gt; attribute, bool allow\_destory, TimePoint tp) <br> |
|  span&lt; const T &gt; | [**view**](#function-view-22) () noexcept const<br>_Get the const attribute values._  |


## Public Functions inherited from uipc::geometry::IAttributeSlot

See [uipc::geometry::IAttributeSlot](classuipc_1_1geometry_1_1_i_attribute_slot.md)

| Type | Name |
| ---: | :--- |
|   | [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-iattributeslot-13) () = default<br> |
|   | [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-iattributeslot-23) (const [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &) = delete<br> |
|   | [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-iattributeslot-33) ([**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &&) noexcept<br> |
|  bool | [**allow\_destroy**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-allow_destroy) () noexcept const<br>_Check if the underlying attribute is allowed to be destroyed._  |
|  bool | [**is\_evolving**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-is_evolving-12) () noexcept const<br> |
|  void | [**is\_evolving**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-is_evolving-22) (bool v) noexcept<br> |
|  bool | [**is\_shared**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-is_shared) () noexcept const<br>_Check if the underlying attribute is shared._  |
|  TimePoint | [**last\_modified**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-last_modified-12) () noexcept const<br>_Get the last modification time of the attribute slot._  |
|  std::string\_view | [**name**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-name) () noexcept const<br>_Get the name of the attribute slot._  |
|  [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) & | [**operator=**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-operator) (const [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &) = delete<br> |
|  [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) & | [**operator=**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-operator_1) ([**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &&) noexcept<br> |
|  SizeT | [**size**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-size) () noexcept const<br> |
|  Json | [**to\_json**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-to_json) () const<br> |
|  std::string\_view | [**type\_name**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-type_name) () noexcept const<br>_Get the type name of data stored in the attribute slot._  |
| virtual  | [**~IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-iattributeslot) () = default<br> |
















































## Protected Functions inherited from uipc::geometry::IAttributeSlot

See [uipc::geometry::IAttributeSlot](classuipc_1_1geometry_1_1_i_attribute_slot.md)

| Type | Name |
| ---: | :--- |
| virtual [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**attribute**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-attribute-12) () noexcept<br> |
| virtual const [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**attribute**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-attribute-22) () noexcept const<br> |
|  S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**clone**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-clone) (std::string\_view name, bool allow\_destroy) const<br> |
|  S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**clone\_empty**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-clone_empty) (std::string\_view name, bool allow\_destroy) const<br> |
| virtual S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**do\_clone**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_clone) (std::string\_view name, bool allow\_destroy) const = 0<br> |
| virtual S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**do\_clone\_empty**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_clone_empty) (std::string\_view name, bool allow\_destroy) const = 0<br> |
| virtual void | [**do\_make\_owned**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_make_owned) () = 0<br> |
| virtual void | [**do\_share\_from**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-do_share_from) (const [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) & other) noexcept = 0<br> |
| virtual bool | [**get\_allow\_destroy**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_allow_destroy) () noexcept const = 0<br> |
| virtual [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**get\_attribute**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_attribute-12) () noexcept = 0<br> |
| virtual const [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**get\_attribute**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_attribute-22) () noexcept const = 0<br> |
| virtual bool | [**get\_is\_evolving**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_is_evolving) () noexcept const = 0<br> |
| virtual TimePoint | [**get\_last\_modified**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_last_modified) () noexcept const = 0<br> |
| virtual std::string\_view | [**get\_name**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_name) () noexcept const = 0<br> |
| virtual SizeT | [**get\_use\_count**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-get_use_count) () const = 0<br> |
|  void | [**last\_modified**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-last_modified-22) (const TimePoint & tp) <br> |
|  void | [**make\_owned**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-make_owned) () <br> |
|  void | [**rw\_access**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-rw_access) () <br> |
| virtual void | [**set\_is\_evolving**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-set_is_evolving) (bool v) noexcept = 0<br> |
| virtual void | [**set\_last\_modified**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-set_last_modified) (const TimePoint & tp) noexcept = 0<br> |
|  void | [**share\_from**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-share_from) (const [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) & other) noexcept<br> |
|  SizeT | [**use\_count**](classuipc_1_1geometry_1_1_i_attribute_slot.md#function-use_count) () const<br> |






## Detailed Description




**Template parameters:**


* `T` The type of the attribute values. 




    
## Public Types Documentation




### typedef value\_type 

```C++
using uipc::geometry::AttributeSlot< T >::value_type =  T;
```




<hr>
## Public Functions Documentation




### function AttributeSlot [1/2]

```C++
uipc::geometry::AttributeSlot::AttributeSlot (
    std::string_view name,
    S< Attribute < T > > attribute,
    bool allow_destroy
) 
```




<hr>



### function AttributeSlot [2/2]

```C++
uipc::geometry::AttributeSlot::AttributeSlot (
    std::string_view name,
    S< Attribute < T > > attribute,
    bool allow_destory,
    TimePoint tp
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

