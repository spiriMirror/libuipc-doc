

# Class uipc::core::AffineBodyStateAccessorFeature



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**AffineBodyStateAccessorFeature**](classuipc_1_1core_1_1AffineBodyStateAccessorFeature.md)








Inherits the following classes: [uipc::core::Feature](classuipc_1_1core_1_1Feature.md)
































## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  constexpr std::string\_view | [**FeatureName**](#variable-featurename)   = `"core/affine\_body\_state\_accessor"`<br> |










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyStateAccessorFeature**](#function-affinebodystateaccessorfeature) (S&lt; [**AffineBodyStateAccessorFeatureOverrider**](classuipc_1_1core_1_1AffineBodyStateAccessorFeatureOverrider.md) &gt; overrider) <br> |
|  SizeT | [**body\_count**](#function-body_count) () const<br>_Get the number of bodies in the affine body system._  |
|  void | [**copy\_from**](#function-copy_from) (const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & state\_geo) const<br>_Copy affine body state data from the given geometry._  |
|  void | [**copy\_to**](#function-copy_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & state\_geo) const<br>_Copy affine body state data to the given geometry._  |
|  void | [**copy\_transform\_to**](#function-copy_transform_to) ([**backend::BufferView**](classuipc_1_1backend_1_1BufferView.md) buffer\_view, IndexT body\_offset=0, SizeT body\_count=~0ull) const<br>_Copy transform data (Matrix4x4) for the specified body range into an externally-owned buffer._  |
|  void | [**copy\_velocity\_to**](#function-copy_velocity_to) ([**backend::BufferView**](classuipc_1_1backend_1_1BufferView.md) buffer\_view, IndexT body\_offset=0, SizeT body\_count=~0ull) const<br>_Copy velocity data (Matrix4x4) for the specified body range into an externally-owned buffer._  |
|  [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**create\_geometry**](#function-create_geometry) (IndexT body\_offset=0, SizeT body\_count=~0ull) <br>_Create a simplicial complex geometry to contain affine body state data._  |




## Public Functions inherited from uipc::core::IFeature

See [uipc::core::IFeature](classuipc_1_1core_1_1IFeature.md)

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**name**](classuipc_1_1core_1_1IFeature.md#function-name) () const<br> |
|  std::string\_view | [**type\_name**](classuipc_1_1core_1_1IFeature.md#function-type_name) () const<br> |
| virtual  | [**~IFeature**](classuipc_1_1core_1_1IFeature.md#function-ifeature) () = default<br> |








































































## Protected Functions inherited from uipc::core::IFeature

See [uipc::core::IFeature](classuipc_1_1core_1_1IFeature.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_on\_required**](classuipc_1_1core_1_1IFeature.md#function-do_on_required) () const = 0<br> |
| virtual std::string\_view | [**get\_name**](classuipc_1_1core_1_1IFeature.md#function-get_name) () const = 0<br> |
| virtual std::string\_view | [**get\_type\_name**](classuipc_1_1core_1_1IFeature.md#function-get_type_name) () const = 0<br> |








## Public Static Attributes Documentation




### variable FeatureName 

```C++
constexpr std::string_view uipc::core::AffineBodyStateAccessorFeature::FeatureName;
```




<hr>
## Public Functions Documentation




### function AffineBodyStateAccessorFeature 

```C++
explicit uipc::core::AffineBodyStateAccessorFeature::AffineBodyStateAccessorFeature (
    S< AffineBodyStateAccessorFeatureOverrider > overrider
) 
```




<hr>



### function body\_count 

_Get the number of bodies in the affine body system._ 
```C++
SizeT uipc::core::AffineBodyStateAccessorFeature::body_count () const
```




<hr>



### function copy\_from 

_Copy affine body state data from the given geometry._ 
```C++
void uipc::core::AffineBodyStateAccessorFeature::copy_from (
    const geometry::SimplicialComplex & state_geo
) const
```





**Parameters:**


* `state_geo` The geometry containing affine body state data to copy from. 




        

<hr>



### function copy\_to 

_Copy affine body state data to the given geometry._ 
```C++
void uipc::core::AffineBodyStateAccessorFeature::copy_to (
    geometry::SimplicialComplex & state_geo
) const
```





**Parameters:**


* `state_geo` The geometry to copy affine body state data to. 




        

<hr>



### function copy\_transform\_to 

_Copy transform data (Matrix4x4) for the specified body range into an externally-owned buffer._ 
```C++
void uipc::core::AffineBodyStateAccessorFeature::copy_transform_to (
    backend::BufferView buffer_view,
    IndexT body_offset=0,
    SizeT body_count=~0ull
) const
```





**Parameters:**


* `buffer_view` The destination buffer view to copy transform data into. 
* `body_offset` The starting body index in affine body system. 
* `body_count` The number of bodies to include, if body\_count == ~0ull, all bodies from body\_offset to the end will be included. 




        

<hr>



### function copy\_velocity\_to 

_Copy velocity data (Matrix4x4) for the specified body range into an externally-owned buffer._ 
```C++
void uipc::core::AffineBodyStateAccessorFeature::copy_velocity_to (
    backend::BufferView buffer_view,
    IndexT body_offset=0,
    SizeT body_count=~0ull
) const
```





**Parameters:**


* `buffer_view` The destination buffer view to copy velocity data into. 
* `body_offset` The starting body index in affine body system. 
* `body_count` The number of bodies to include, if body\_count == ~0ull, all bodies from body\_offset to the end will be included. 




        

<hr>



### function create\_geometry 

_Create a simplicial complex geometry to contain affine body state data._ 
```C++
geometry::SimplicialComplex uipc::core::AffineBodyStateAccessorFeature::create_geometry (
    IndexT body_offset=0,
    SizeT body_count=~0ull
) 
```





**Parameters:**


* `body_offset` The starting body index in affine body system. 
* `body_count` The number of bodies to include, if body\_count == ~0ull, all bodies from body\_offset to the end will be included. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/affine_body_state_accessor_feature.h`

