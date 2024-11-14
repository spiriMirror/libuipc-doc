

# Class uipc::geometry::Geometry::InstanceAttributesT

**template &lt;bool IsConst&gt;**



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) **>** [**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md)



_A wrapper class for the instance attributes of a geometries._ 

* `#include <geometry.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**InstanceAttributesT**](#function-instanceattributest-24) (AutoAttributeCollection & attributes) <br> |
|   | [**InstanceAttributesT**](#function-instanceattributest-34) (const [**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) & o) = default<br> |
|   | [**InstanceAttributesT**](#function-instanceattributest-44) ([**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) && o) = default<br> |
|  void | [**clear**](#function-clear) () <br> |
|  void | [**copy\_from**](#function-copy_from) ([**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md)&lt; true &gt; other, const [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md) & copy={}, span&lt; const string &gt; include\_names={}, span&lt; const string &gt; exclude\_names={}) <br> |
|  decltype(auto) | [**create**](#function-create) (std::string\_view name, const T & init\_value={}) <br>_Create an attribute with the given name._  |
|  void | [**destroy**](#function-destroy) (std::string\_view name) <br> |
|  auto | [**find**](#function-find) (std::string\_view name) <br>_Find an attribute by type and name, if the attribute does not exist, return nullptr._  |
|  [**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) & | [**operator=**](#function-operator) (const [**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) & o) = default<br> |
|  [**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) & | [**operator=**](#function-operator_1) ([**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) && o) = default<br> |
|  void | [**reserve**](#function-reserve) (size\_t size) <br> |
|  void | [**resize**](#function-resize) (size\_t size) <br> |
|  decltype(auto) | [**share**](#function-share) (std::string\_view name, const [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; T &gt; & slot) <br> |
|  SizeT | [**size**](#function-size) () <br> |
|  Json | [**to\_json**](#function-to_json) () const<br> |




























## Public Functions Documentation




### function InstanceAttributesT [2/4]

```C++
inline uipc::geometry::Geometry::InstanceAttributesT::InstanceAttributesT (
    AutoAttributeCollection & attributes
) 
```




<hr>



### function InstanceAttributesT [3/4]

```C++
uipc::geometry::Geometry::InstanceAttributesT::InstanceAttributesT (
    const InstanceAttributesT & o
) = default
```




<hr>



### function InstanceAttributesT [4/4]

```C++
uipc::geometry::Geometry::InstanceAttributesT::InstanceAttributesT (
    InstanceAttributesT && o
) = default
```




<hr>



### function clear 


```C++
void uipc::geometry::Geometry::InstanceAttributesT::clear () 
```





**See also:** [**AttributeCollection::clear**](classuipc_1_1geometry_1_1_attribute_collection.md#function-clear) 



        

<hr>



### function copy\_from 

```C++
inline void uipc::geometry::Geometry::InstanceAttributesT::copy_from (
    InstanceAttributesT < true > other,
    const AttributeCopy & copy={},
    span< const string > include_names={},
    span< const string > exclude_names={}
) 
```




<hr>



### function create 

```C++
template<typename T>
inline decltype(auto) uipc::geometry::Geometry::InstanceAttributesT::create (
    std::string_view name,
    const T & init_value={}
) 
```




<hr>



### function destroy 


```C++
void uipc::geometry::Geometry::InstanceAttributesT::destroy (
    std::string_view name
) 
```





**See also:** [**AttributeCollection::destroy**](classuipc_1_1geometry_1_1_attribute_collection.md#function-destroy) 



        

<hr>



### function find 

```C++
template<typename T>
inline auto uipc::geometry::Geometry::InstanceAttributesT::find (
    std::string_view name
) 
```




<hr>



### function operator= 

```C++
InstanceAttributesT & uipc::geometry::Geometry::InstanceAttributesT::operator= (
    const InstanceAttributesT & o
) = default
```




<hr>



### function operator= 

```C++
InstanceAttributesT & uipc::geometry::Geometry::InstanceAttributesT::operator= (
    InstanceAttributesT && o
) = default
```




<hr>



### function reserve 


```C++
void uipc::geometry::Geometry::InstanceAttributesT::reserve (
    size_t size
) 
```





**See also:** [**AttributeCollection::reserve**](classuipc_1_1geometry_1_1_attribute_collection.md#function-reserve) 



        

<hr>



### function resize 


```C++
void uipc::geometry::Geometry::InstanceAttributesT::resize (
    size_t size
) 
```





**See also:** [**AttributeCollection::resize**](classuipc_1_1geometry_1_1_attribute_collection.md#function-resize) 



        

<hr>



### function share 

```C++
template<typename T>
inline decltype(auto) uipc::geometry::Geometry::InstanceAttributesT::share (
    std::string_view name,
    const AttributeSlot < T > & slot
) 
```




<hr>



### function size 


```C++
SizeT uipc::geometry::Geometry::InstanceAttributesT::size () 
```





**See also:** [**AttributeCollection::size**](classuipc_1_1geometry_1_1_attribute_collection.md#function-size) 



        

<hr>



### function to\_json 

```C++
Json uipc::geometry::Geometry::InstanceAttributesT::to_json () const
```




<hr>## Friends Documentation





### friend formatter&lt; InstanceAttributesT&lt; IsConst &gt; &gt; 

```C++
struct uipc::geometry::Geometry::InstanceAttributesT::formatter< InstanceAttributesT< IsConst > > (
    fmt::formatter< InstanceAttributesT < IsConst > >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry.h`

