

# Class uipc::geometry::IAttributeSlot



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md)



_An abstract class to represent a geometries attribute slot in a geometries attribute collection._ 

* `#include <attribute_slot.h>`





Inherited by the following classes: [uipc::geometry::AttributeSlot](classuipc_1_1geometry_1_1_attribute_slot.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**IAttributeSlot**](#function-iattributeslot-13) () = default<br> |
|   | [**IAttributeSlot**](#function-iattributeslot-23) (const [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &) = delete<br> |
|   | [**IAttributeSlot**](#function-iattributeslot-33) ([**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &&) noexcept<br> |
|  bool | [**allow\_destroy**](#function-allow_destroy) () noexcept const<br>_Check if the underlying attribute is allowed to be destroyed._  |
|  bool | [**is\_evolving**](#function-is_evolving-12) () noexcept const<br> |
|  void | [**is\_evolving**](#function-is_evolving-22) (bool v) noexcept<br> |
|  bool | [**is\_shared**](#function-is_shared) () noexcept const<br>_Check if the underlying attribute is shared._  |
|  TimePoint | [**last\_modified**](#function-last_modified) () noexcept const<br>_Get the last modification time of the attribute slot._  |
|  std::string\_view | [**name**](#function-name) () noexcept const<br>_Get the name of the attribute slot._  |
|  [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) & | [**operator=**](#function-operator) (const [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &) = delete<br> |
|  [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) & | [**operator=**](#function-operator_1) ([**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &&) noexcept<br> |
|  SizeT | [**size**](#function-size) () noexcept const<br> |
|  Json | [**to\_json**](#function-to_json) () const<br> |
|  std::string\_view | [**type\_name**](#function-type_name) () noexcept const<br>_Get the type name of data stored in the attribute slot._  |
| virtual  | [**~IAttributeSlot**](#function-iattributeslot) () = default<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**attribute**](#function-attribute-12) () noexcept<br> |
| virtual const [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**attribute**](#function-attribute-22) () noexcept const<br> |
|  S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**clone**](#function-clone) (std::string\_view name, bool allow\_destroy) const<br> |
|  S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**clone\_empty**](#function-clone_empty) (std::string\_view name, bool allow\_destroy) const<br> |
| virtual S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**do\_clone**](#function-do_clone) (std::string\_view name, bool allow\_destroy) const = 0<br> |
| virtual S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; | [**do\_clone\_empty**](#function-do_clone_empty) (std::string\_view name, bool allow\_destroy) const = 0<br> |
| virtual void | [**do\_make\_owned**](#function-do_make_owned) () = 0<br> |
| virtual void | [**do\_share\_from**](#function-do_share_from) (const [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) & other) noexcept = 0<br> |
| virtual bool | [**get\_allow\_destroy**](#function-get_allow_destroy) () noexcept const = 0<br> |
| virtual [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**get\_attribute**](#function-get_attribute-12) () noexcept = 0<br> |
| virtual const [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) & | [**get\_attribute**](#function-get_attribute-22) () noexcept const = 0<br> |
| virtual bool | [**get\_is\_evolving**](#function-get_is_evolving) () noexcept const = 0<br> |
| virtual TimePoint | [**get\_last\_modified**](#function-get_last_modified) () noexcept const = 0<br> |
| virtual std::string\_view | [**get\_name**](#function-get_name) () noexcept const = 0<br> |
| virtual SizeT | [**get\_use\_count**](#function-get_use_count) () const = 0<br> |
|  void | [**make\_owned**](#function-make_owned) () <br> |
| virtual void | [**set\_is\_evolving**](#function-set_is_evolving) (bool v) noexcept = 0<br> |
|  void | [**share\_from**](#function-share_from) (const [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) & other) noexcept<br> |
|  SizeT | [**use\_count**](#function-use_count) () const<br> |




## Public Functions Documentation




### function IAttributeSlot [1/3]

```C++
uipc::geometry::IAttributeSlot::IAttributeSlot () = default
```




<hr>



### function IAttributeSlot [2/3]

```C++
uipc::geometry::IAttributeSlot::IAttributeSlot (
    const IAttributeSlot &
) = delete
```




<hr>



### function IAttributeSlot [3/3]

```C++
uipc::geometry::IAttributeSlot::IAttributeSlot (
    IAttributeSlot &&
) noexcept
```




<hr>



### function allow\_destroy 

_Check if the underlying attribute is allowed to be destroyed._ 
```C++
bool uipc::geometry::IAttributeSlot::allow_destroy () noexcept const
```




<hr>



### function is\_evolving [1/2]

```C++
bool uipc::geometry::IAttributeSlot::is_evolving () noexcept const
```




<hr>



### function is\_evolving [2/2]

```C++
void uipc::geometry::IAttributeSlot::is_evolving (
    bool v
) noexcept
```




<hr>



### function is\_shared 

_Check if the underlying attribute is shared._ 
```C++
bool uipc::geometry::IAttributeSlot::is_shared () noexcept const
```





**Returns:**

true, if the underlying attribute is shared, more than one geometries reference to the underlying attribute. 




**Returns:**

false, if the underlying attribute is owned, only this geometries reference to the underlying attribute. 





        

<hr>



### function last\_modified 

_Get the last modification time of the attribute slot._ 
```C++
TimePoint uipc::geometry::IAttributeSlot::last_modified () noexcept const
```




<hr>



### function name 

_Get the name of the attribute slot._ 
```C++
std::string_view uipc::geometry::IAttributeSlot::name () noexcept const
```




<hr>



### function operator= 

```C++
IAttributeSlot & uipc::geometry::IAttributeSlot::operator= (
    const IAttributeSlot &
) = delete
```




<hr>



### function operator= 

```C++
IAttributeSlot & uipc::geometry::IAttributeSlot::operator= (
    IAttributeSlot &&
) noexcept
```




<hr>



### function size 

```C++
SizeT uipc::geometry::IAttributeSlot::size () noexcept const
```




<hr>



### function to\_json 

```C++
Json uipc::geometry::IAttributeSlot::to_json () const
```




<hr>



### function type\_name 

_Get the type name of data stored in the attribute slot._ 
```C++
std::string_view uipc::geometry::IAttributeSlot::type_name () noexcept const
```




<hr>



### function ~IAttributeSlot 

```C++
virtual uipc::geometry::IAttributeSlot::~IAttributeSlot () = default
```




<hr>
## Protected Functions Documentation




### function attribute [1/2]

```C++
virtual IAttribute & uipc::geometry::IAttributeSlot::attribute () noexcept
```




<hr>



### function attribute [2/2]

```C++
virtual const IAttribute & uipc::geometry::IAttributeSlot::attribute () noexcept const
```




<hr>



### function clone 

```C++
S< IAttributeSlot > uipc::geometry::IAttributeSlot::clone (
    std::string_view name,
    bool allow_destroy
) const
```




<hr>



### function clone\_empty 

```C++
S< IAttributeSlot > uipc::geometry::IAttributeSlot::clone_empty (
    std::string_view name,
    bool allow_destroy
) const
```




<hr>



### function do\_clone 

```C++
virtual S< IAttributeSlot > uipc::geometry::IAttributeSlot::do_clone (
    std::string_view name,
    bool allow_destroy
) const = 0
```




<hr>



### function do\_clone\_empty 

```C++
virtual S< IAttributeSlot > uipc::geometry::IAttributeSlot::do_clone_empty (
    std::string_view name,
    bool allow_destroy
) const = 0
```




<hr>



### function do\_make\_owned 

```C++
virtual void uipc::geometry::IAttributeSlot::do_make_owned () = 0
```




<hr>



### function do\_share\_from 

```C++
virtual void uipc::geometry::IAttributeSlot::do_share_from (
    const IAttributeSlot & other
) noexcept = 0
```




<hr>



### function get\_allow\_destroy 

```C++
virtual bool uipc::geometry::IAttributeSlot::get_allow_destroy () noexcept const = 0
```




<hr>



### function get\_attribute [1/2]

```C++
virtual IAttribute & uipc::geometry::IAttributeSlot::get_attribute () noexcept = 0
```




<hr>



### function get\_attribute [2/2]

```C++
virtual const IAttribute & uipc::geometry::IAttributeSlot::get_attribute () noexcept const = 0
```




<hr>



### function get\_is\_evolving 

```C++
virtual bool uipc::geometry::IAttributeSlot::get_is_evolving () noexcept const = 0
```




<hr>



### function get\_last\_modified 

```C++
virtual TimePoint uipc::geometry::IAttributeSlot::get_last_modified () noexcept const = 0
```




<hr>



### function get\_name 

```C++
virtual std::string_view uipc::geometry::IAttributeSlot::get_name () noexcept const = 0
```




<hr>



### function get\_use\_count 

```C++
virtual SizeT uipc::geometry::IAttributeSlot::get_use_count () const = 0
```




<hr>



### function make\_owned 

```C++
void uipc::geometry::IAttributeSlot::make_owned () 
```




<hr>



### function set\_is\_evolving 

```C++
virtual void uipc::geometry::IAttributeSlot::set_is_evolving (
    bool v
) noexcept = 0
```




<hr>



### function share\_from 

```C++
void uipc::geometry::IAttributeSlot::share_from (
    const IAttributeSlot & other
) noexcept
```




<hr>



### function use\_count 

```C++
SizeT uipc::geometry::IAttributeSlot::use_count () const
```




<hr>## Friends Documentation





### friend AttributeFriend 

```C++
template<typename T>
class uipc::geometry::IAttributeSlot::AttributeFriend (
    AttributeFriend
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/attribute_slot.h`

