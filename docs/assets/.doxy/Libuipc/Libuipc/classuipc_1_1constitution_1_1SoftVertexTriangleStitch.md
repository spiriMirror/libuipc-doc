

# Class uipc::constitution::SoftVertexTriangleStitch



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**SoftVertexTriangleStitch**](classuipc_1_1constitution_1_1SoftVertexTriangleStitch.md)



_Inter-primitive constitution: (vertex, triangle) pairs form tetrahedra with_ [_**StableNeoHookean**_](classuipc_1_1constitution_1_1StableNeoHookean.md) _energy. UID = 30._

* `#include <soft_vertex_triangle_stitch.h>`



Inherits the following classes: [uipc::constitution::InterPrimitiveConstitution](classuipc_1_1constitution_1_1InterPrimitiveConstitution.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::tuple&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt;, S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; | [**SlotTuple**](#typedef-slottuple)  <br> |




























































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SoftVertexTriangleStitch**](#function-softvertextrianglestitch) (const Json & config=default\_config()) <br> |
|  [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) | [**create\_geometry**](#function-create_geometry-12) (const SlotTuple & aim\_geo\_slots, const SlotTuple & rest\_geo\_slots, span&lt; const Vector2i &gt; stitched\_vert\_tri\_ids, const [**ElasticModuli**](classuipc_1_1constitution_1_1ElasticModuli.md) & moduli=ElasticModuli::youngs\_poisson(120.0\_kPa, 0.49), Float min\_separate\_distance=0.001) const<br>_Create stitch geometry from explicit (vertex\_index, triangle\_index) pairs. When a tet is degenerate, rest vertex is offset by min\_separate\_distance (default 1 mm)._  |
|  [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) | [**create\_geometry**](#function-create_geometry-22) (const SlotTuple & aim\_geo\_slots, const SlotTuple & rest\_geo\_slots, const [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & pair\_geometry, const [**ElasticModuli**](classuipc_1_1constitution_1_1ElasticModuli.md) & moduli=ElasticModuli::youngs\_poisson(120.0\_kPa, 0.49), Float min\_separate\_distance=0.001) const<br>_Create stitch geometry from the Geometry returned by closest\_vertex\_triangle\_pairs. When a tet is degenerate, uses min\_separate\_distance (default 1 mm)._  |




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




### typedef SlotTuple 

```C++
using uipc::constitution::SoftVertexTriangleStitch::SlotTuple =  std::tuple<S<geometry::SimplicialComplexSlot>, S<geometry::SimplicialComplexSlot> >;
```




<hr>
## Public Functions Documentation




### function SoftVertexTriangleStitch 

```C++
uipc::constitution::SoftVertexTriangleStitch::SoftVertexTriangleStitch (
    const Json & config=default_config()
) 
```




<hr>



### function create\_geometry [1/2]

_Create stitch geometry from explicit (vertex\_index, triangle\_index) pairs. When a tet is degenerate, rest vertex is offset by min\_separate\_distance (default 1 mm)._ 
```C++
geometry::Geometry uipc::constitution::SoftVertexTriangleStitch::create_geometry (
    const SlotTuple & aim_geo_slots,
    const SlotTuple & rest_geo_slots,
    span< const Vector2i > stitched_vert_tri_ids,
    const ElasticModuli & moduli=ElasticModuli::youngs_poisson(120.0_kPa, 0.49),
    Float min_separate_distance=0.001
) const
```




<hr>



### function create\_geometry [2/2]

_Create stitch geometry from the Geometry returned by closest\_vertex\_triangle\_pairs. When a tet is degenerate, uses min\_separate\_distance (default 1 mm)._ 
```C++
geometry::Geometry uipc::constitution::SoftVertexTriangleStitch::create_geometry (
    const SlotTuple & aim_geo_slots,
    const SlotTuple & rest_geo_slots,
    const geometry::Geometry & pair_geometry,
    const ElasticModuli & moduli=ElasticModuli::youngs_poisson(120.0_kPa, 0.49),
    Float min_separate_distance=0.001
) const
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::SoftVertexTriangleStitch::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/soft_vertex_triangle_stitch.h`

