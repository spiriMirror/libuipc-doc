

# Class uipc::geometry::Geometry::MetaAttributesT

**template &lt;bool IsConst&gt;**



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) **>** [**MetaAttributesT**](classuipc_1_1geometry_1_1Geometry_1_1MetaAttributesT.md)



_A wrapper class for the meta attributes of a geometries._ 

* `#include <geometry.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**MetaAttributesT**](#function-metaattributest-25) (AutoAttributeCollection & attributes) <br> |
|   | [**MetaAttributesT**](#function-metaattributest-35) (const [**MetaAttributesT**](classuipc_1_1geometry_1_1Geometry_1_1MetaAttributesT.md)&lt; OtherIsConst &gt; & o) noexcept<br> |
|   | [**MetaAttributesT**](#function-metaattributest-45) (const [**MetaAttributesT**](classuipc_1_1geometry_1_1Geometry_1_1MetaAttributesT.md) & o) = default<br> |
|   | [**MetaAttributesT**](#function-metaattributest-55) ([**MetaAttributesT**](classuipc_1_1geometry_1_1Geometry_1_1MetaAttributesT.md) && o) = default<br> |
|  void | [**copy\_from**](#function-copy_from) ([**MetaAttributesT**](classuipc_1_1geometry_1_1Geometry_1_1MetaAttributesT.md)&lt; true &gt; other, const [**AttributeCopy**](classuipc_1_1geometry_1_1AttributeCopy.md) & copy={}, span&lt; const string &gt; include\_names={}, span&lt; const string &gt; exclude\_names={}) <br> |
|  decltype(auto) | [**create**](#function-create) (std::string\_view name, const T & init\_value={}) <br>_Create an attribute with the given name._  |
|  void | [**destroy**](#function-destroy) (std::string\_view name) <br> |
|  auto | [**find**](#function-find) (std::string\_view name) <br>_Find an attribute by type and name, if the attribute does not exist, return nullptr._  |
|  [**MetaAttributesT**](classuipc_1_1geometry_1_1Geometry_1_1MetaAttributesT.md) & | [**operator=**](#function-operator) (const [**MetaAttributesT**](classuipc_1_1geometry_1_1Geometry_1_1MetaAttributesT.md) & o) = default<br> |
|  [**MetaAttributesT**](classuipc_1_1geometry_1_1Geometry_1_1MetaAttributesT.md) & | [**operator=**](#function-operator_1) ([**MetaAttributesT**](classuipc_1_1geometry_1_1Geometry_1_1MetaAttributesT.md) && o) = default<br> |
|  decltype(auto) | [**share**](#function-share) (std::string\_view name, const [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; T &gt; & slot) <br> |
|  Json | [**to\_json**](#function-to_json) () const<br> |




























## Public Functions Documentation




### function MetaAttributesT [2/5]

```C++
inline uipc::geometry::Geometry::MetaAttributesT::MetaAttributesT (
    AutoAttributeCollection & attributes
) 
```




<hr>



### function MetaAttributesT [3/5]

```C++
template<bool OtherIsConst>
inline uipc::geometry::Geometry::MetaAttributesT::MetaAttributesT (
    const MetaAttributesT < OtherIsConst > & o
) noexcept
```




<hr>



### function MetaAttributesT [4/5]

```C++
uipc::geometry::Geometry::MetaAttributesT::MetaAttributesT (
    const MetaAttributesT & o
) = default
```




<hr>



### function MetaAttributesT [5/5]

```C++
uipc::geometry::Geometry::MetaAttributesT::MetaAttributesT (
    MetaAttributesT && o
) = default
```




<hr>



### function copy\_from 

```C++
inline void uipc::geometry::Geometry::MetaAttributesT::copy_from (
    MetaAttributesT < true > other,
    const AttributeCopy & copy={},
    span< const string > include_names={},
    span< const string > exclude_names={}
) 
```




<hr>



### function create 

_Create an attribute with the given name._ 
```C++
template<typename T>
inline decltype(auto) uipc::geometry::Geometry::MetaAttributesT::create (
    std::string_view name,
    const T & init_value={}
) 
```




<hr>



### function destroy 

```C++
inline void uipc::geometry::Geometry::MetaAttributesT::destroy (
    std::string_view name
) 
```





**See also:** [**AttributeCollection::destroy**](classuipc_1_1geometry_1_1AttributeCollection.md#function-destroy) 



        

<hr>



### function find 

_Find an attribute by type and name, if the attribute does not exist, return nullptr._ 
```C++
template<typename T>
inline auto uipc::geometry::Geometry::MetaAttributesT::find (
    std::string_view name
) 
```




<hr>



### function operator= 

```C++
MetaAttributesT & uipc::geometry::Geometry::MetaAttributesT::operator= (
    const MetaAttributesT & o
) = default
```




<hr>



### function operator= 

```C++
MetaAttributesT & uipc::geometry::Geometry::MetaAttributesT::operator= (
    MetaAttributesT && o
) = default
```




<hr>



### function share 

```C++
template<typename T>
inline decltype(auto) uipc::geometry::Geometry::MetaAttributesT::share (
    std::string_view name,
    const AttributeSlot < T > & slot
) 
```




<hr>



### function to\_json 

```C++
Json uipc::geometry::Geometry::MetaAttributesT::to_json () const
```




<hr>## Friends Documentation





### friend formatter&lt; MetaAttributesT&lt; IsConst &gt; &gt; 

```C++
struct uipc::geometry::Geometry::MetaAttributesT::formatter< MetaAttributesT< IsConst > > (
    fmt::formatter< MetaAttributesT < IsConst > >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry.h`

