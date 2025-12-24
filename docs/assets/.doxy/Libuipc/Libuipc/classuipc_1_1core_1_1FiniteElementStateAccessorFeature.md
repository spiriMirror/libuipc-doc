

# Class uipc::core::FiniteElementStateAccessorFeature



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**FiniteElementStateAccessorFeature**](classuipc_1_1core_1_1FiniteElementStateAccessorFeature.md)



[_**Feature**_](classuipc_1_1core_1_1Feature.md) _to access finite element state data._[More...](#detailed-description)

* `#include <finite_element_state_accessor_feature.h>`



Inherits the following classes: [uipc::core::Feature](classuipc_1_1core_1_1Feature.md)
































## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  constexpr std::string\_view | [**FeatureName**](#variable-featurename)   = `"core/finite\_element\_state\_accessor"`<br> |










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FiniteElementStateAccessorFeature**](#function-finiteelementstateaccessorfeature) (S&lt; [**FiniteElementStateAccessorFeatureOverrider**](classuipc_1_1core_1_1FiniteElementStateAccessorFeatureOverrider.md) &gt; overrider) <br> |
|  void | [**copy\_from**](#function-copy_from) (const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & state\_geo) const<br>_Copy finite element state data from the given geometry._  |
|  void | [**copy\_to**](#function-copy_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & state\_geo) const<br>_Copy finite element state data to the given geometry._  |
|  [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**create\_geometry**](#function-create_geometry) (IndexT vertex\_offset=0, SizeT vertex\_count=~0ull) const<br>_Create a simplicial complex geometry to contain finite element state data._  |
|  SizeT | [**vertex\_count**](#function-vertex_count) () const<br>_Get the number of vertices in the finite element system._  |




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








## Detailed Description


[https://github.com/spiriMirror/libuipc/discussions/232](https://github.com/spiriMirror/libuipc/discussions/232) 


    
## Public Static Attributes Documentation




### variable FeatureName 

```C++
constexpr std::string_view uipc::core::FiniteElementStateAccessorFeature::FeatureName;
```




<hr>
## Public Functions Documentation




### function FiniteElementStateAccessorFeature 

```C++
explicit uipc::core::FiniteElementStateAccessorFeature::FiniteElementStateAccessorFeature (
    S< FiniteElementStateAccessorFeatureOverrider > overrider
) 
```




<hr>



### function copy\_from 

_Copy finite element state data from the given geometry._ 
```C++
void uipc::core::FiniteElementStateAccessorFeature::copy_from (
    const geometry::SimplicialComplex & state_geo
) const
```





**Parameters:**


* `state_geo` The geometry containing finite element state data to copy from. 




        

<hr>



### function copy\_to 

_Copy finite element state data to the given geometry._ 
```C++
void uipc::core::FiniteElementStateAccessorFeature::copy_to (
    geometry::SimplicialComplex & state_geo
) const
```





**Parameters:**


* `state_geo` The geometry to copy finite element state data to. 




        

<hr>



### function create\_geometry 

_Create a simplicial complex geometry to contain finite element state data._ 
```C++
geometry::SimplicialComplex uipc::core::FiniteElementStateAccessorFeature::create_geometry (
    IndexT vertex_offset=0,
    SizeT vertex_count=~0ull
) const
```





**Parameters:**


* `vertex_offset` The starting vertex index in finite element system. 
* `vertex_count` The number of vertices to include, if vertex\_count == ~0ull, all vertices from vertex\_offset to the end will be included. 




        

<hr>



### function vertex\_count 

_Get the number of vertices in the finite element system._ 
```C++
SizeT uipc::core::FiniteElementStateAccessorFeature::vertex_count () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/finite_element_state_accessor_feature.h`

