

# Class uipc::constitution::SoftVertexStitch



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**SoftVertexStitch**](classuipc_1_1constitution_1_1SoftVertexStitch.md)








Inherits the following classes: [uipc::constitution::InterPrimitiveConstitution](classuipc_1_1constitution_1_1InterPrimitiveConstitution.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::tuple&lt; [**core::ContactElement**](classuipc_1_1core_1_1ContactElement.md), [**core::ContactElement**](classuipc_1_1core_1_1ContactElement.md) &gt; | [**ContactElementTuple**](#typedef-contactelementtuple)  <br> |
| typedef std::tuple&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt;, S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; | [**SlotTuple**](#typedef-slottuple)  <br> |




























































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SoftVertexStitch**](#function-softvertexstitch) (const Json & config=default\_config()) <br> |
|  [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) | [**create\_geometry**](#function-create_geometry-12) (const SlotTuple & aim\_geo\_slots, span&lt; const Vector2i &gt; stitched\_vert\_ids, Float kappa=1e6) const<br>_Create soft vertex stitch constraints between two Geometries._  |
|  [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) | [**create\_geometry**](#function-create_geometry-22) (const SlotTuple & aim\_geo\_slots, span&lt; const Vector2i &gt; stitched\_vert\_ids, const ContactElementTuple & contact\_elements, Float kappa=1e6) const<br> |




## Public Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**name**](classuipc_1_1constitution_1_1IConstitution.md#function-name) () noexcept const<br> |
|  std::string\_view | [**type**](classuipc_1_1constitution_1_1IConstitution.md#function-type) () noexcept const<br> |
|  U64 | [**uid**](classuipc_1_1constitution_1_1IConstitution.md#function-uid) () noexcept const<br> |
|  const [**builtin::UIDInfo**](structuipc_1_1builtin_1_1UIDInfo.md) & | [**uid\_info**](classuipc_1_1constitution_1_1IConstitution.md#function-uid_info) () noexcept const<br> |
| virtual  | [**~IConstitution**](classuipc_1_1constitution_1_1IConstitution.md#function-iconstitution) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Json | [**default\_config**](#function-default_config) () <br> |






































































## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid) () noexcept const = 0<br> |








## Public Types Documentation




### typedef ContactElementTuple 

```C++
using uipc::constitution::SoftVertexStitch::ContactElementTuple =  std::tuple<core::ContactElement, core::ContactElement>;
```




<hr>



### typedef SlotTuple 

```C++
using uipc::constitution::SoftVertexStitch::SlotTuple =  std::tuple<S<geometry::SimplicialComplexSlot>, S<geometry::SimplicialComplexSlot> >;
```




<hr>
## Public Functions Documentation




### function SoftVertexStitch 

```C++
uipc::constitution::SoftVertexStitch::SoftVertexStitch (
    const Json & config=default_config()
) 
```




<hr>



### function create\_geometry [1/2]

_Create soft vertex stitch constraints between two Geometries._ 
```C++
geometry::Geometry uipc::constitution::SoftVertexStitch::create_geometry (
    const SlotTuple & aim_geo_slots,
    span< const Vector2i > stitched_vert_ids,
    Float kappa=1e6
) const
```





**Parameters:**


* `aim_geo_slots` The slots of the two geometries to be stitched 
* `stitched_vert_ids` Each element is a pair of vertex ids, the first one is from the first geometry, the second one is from the second geometry 
* `kappa` The stiffness of the stitch constraint 




        

<hr>



### function create\_geometry [2/2]

```C++
geometry::Geometry uipc::constitution::SoftVertexStitch::create_geometry (
    const SlotTuple & aim_geo_slots,
    span< const Vector2i > stitched_vert_ids,
    const ContactElementTuple & contact_elements,
    Float kappa=1e6
) const
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::SoftVertexStitch::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/soft_vertex_stitch.h`

