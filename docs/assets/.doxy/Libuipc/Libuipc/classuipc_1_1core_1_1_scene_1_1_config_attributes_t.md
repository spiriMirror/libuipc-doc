

# Class uipc::core::Scene::ConfigAttributesT

**template &lt;bool IsConst&gt;**



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**Scene**](classuipc_1_1core_1_1_scene.md) **>** [**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ConfigAttributesT**](#function-configattributest-25) (AutoAttributeCollection & attributes) <br> |
|   | [**ConfigAttributesT**](#function-configattributest-35) (const [**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md)&lt; OtherIsConst &gt; & o) noexcept<br> |
|   | [**ConfigAttributesT**](#function-configattributest-45) (const [**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md) & o) = default<br> |
|   | [**ConfigAttributesT**](#function-configattributest-55) ([**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md) && o) = default<br> |
|  void | [**copy\_from**](#function-copy_from) ([**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md)&lt; true &gt; other, const [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md) & copy={}, span&lt; const string &gt; include\_names={}, span&lt; const string &gt; exclude\_names={}) <br> |
|  decltype(auto) | [**create**](#function-create) (std::string\_view name, const T & init\_value={}) <br>_Create an attribute with the given name._  |
|  void | [**destroy**](#function-destroy) (std::string\_view name) <br> |
|  auto | [**find**](#function-find) (std::string\_view name) <br>_Find an attribute by type and name, if the attribute does not exist, return nullptr._  |
|  [**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md) & | [**operator=**](#function-operator) (const [**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md) & o) = default<br> |
|  [**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md) & | [**operator=**](#function-operator_1) ([**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md) && o) = default<br> |
|  decltype(auto) | [**share**](#function-share) (std::string\_view name, const [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; T &gt; & slot) <br> |
|  Json | [**to\_json**](#function-to_json) () const<br> |




























## Public Functions Documentation




### function ConfigAttributesT [2/5]

```C++
inline uipc::core::Scene::ConfigAttributesT::ConfigAttributesT (
    AutoAttributeCollection & attributes
) 
```




<hr>



### function ConfigAttributesT [3/5]

```C++
template<bool OtherIsConst>
inline uipc::core::Scene::ConfigAttributesT::ConfigAttributesT (
    const ConfigAttributesT < OtherIsConst > & o
) noexcept
```




<hr>



### function ConfigAttributesT [4/5]

```C++
uipc::core::Scene::ConfigAttributesT::ConfigAttributesT (
    const ConfigAttributesT & o
) = default
```




<hr>



### function ConfigAttributesT [5/5]

```C++
uipc::core::Scene::ConfigAttributesT::ConfigAttributesT (
    ConfigAttributesT && o
) = default
```




<hr>



### function copy\_from 

```C++
inline void uipc::core::Scene::ConfigAttributesT::copy_from (
    ConfigAttributesT < true > other,
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
inline decltype(auto) uipc::core::Scene::ConfigAttributesT::create (
    std::string_view name,
    const T & init_value={}
) 
```




<hr>



### function destroy 

```C++
inline void uipc::core::Scene::ConfigAttributesT::destroy (
    std::string_view name
) 
```





**See also:** [**AttributeCollection::destroy**](classuipc_1_1geometry_1_1_attribute_collection.md#function-destroy) 



        

<hr>



### function find 

_Find an attribute by type and name, if the attribute does not exist, return nullptr._ 
```C++
template<typename T>
inline auto uipc::core::Scene::ConfigAttributesT::find (
    std::string_view name
) 
```




<hr>



### function operator= 

```C++
ConfigAttributesT & uipc::core::Scene::ConfigAttributesT::operator= (
    const ConfigAttributesT & o
) = default
```




<hr>



### function operator= 

```C++
ConfigAttributesT & uipc::core::Scene::ConfigAttributesT::operator= (
    ConfigAttributesT && o
) = default
```




<hr>



### function share 

```C++
template<typename T>
inline decltype(auto) uipc::core::Scene::ConfigAttributesT::share (
    std::string_view name,
    const AttributeSlot < T > & slot
) 
```




<hr>



### function to\_json 

```C++
inline Json uipc::core::Scene::ConfigAttributesT::to_json () const
```




<hr>## Friends Documentation





### friend formatter&lt; ConfigAttributesT&lt; IsConst &gt; &gt; 

```C++
struct uipc::core::Scene::ConfigAttributesT::formatter< ConfigAttributesT< IsConst > > (
    fmt::formatter< ConfigAttributesT < IsConst > >
) 
```




<hr>



### friend AttributeFriend 

```C++
template<typename T>
class uipc::core::Scene::ConfigAttributesT::AttributeFriend (
    geometry::AttributeFriend
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/scene.h`

