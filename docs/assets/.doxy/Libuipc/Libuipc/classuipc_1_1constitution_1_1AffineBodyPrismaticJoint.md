

# Class uipc::constitution::AffineBodyPrismaticJoint



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodyPrismaticJoint**](classuipc_1_1constitution_1_1AffineBodyPrismaticJoint.md)








Inherits the following classes: [uipc::constitution::InterAffineBodyConstitution](classuipc_1_1constitution_1_1InterAffineBodyConstitution.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::tuple&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt;, S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; | [**SlotTuple**](#typedef-slottuple)  <br> |




























































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyPrismaticJoint**](#function-affinebodyprismaticjoint) (const Json & config=default\_config()) <br> |
|  void | [**apply\_to**](#function-apply_to-13) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & edges, span&lt; SlotTuple &gt; geo\_slots, Float strength\_ratio=Float{100}) <br>_Deprecated: Apply prismatic joint to edges connecting affine bodies._  |
|  void | [**apply\_to**](#function-apply_to-23) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & edges, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; l\_geo\_slots, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; r\_geo\_slots, Float strength\_ratio=Float{100}) <br>_Apply prismatic joint to edges connecting affine bodies (single-instance mode)._  |
|  void | [**apply\_to**](#function-apply_to-33) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & edges, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; l\_geo\_slots, span&lt; IndexT &gt; l\_instance\_id, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; r\_geo\_slots, span&lt; IndexT &gt; r\_instance\_id, span&lt; Float &gt; strength\_ratio) <br>_Apply prismatic joint to edges connecting affine bodies (multi-instance mode)._  |
| virtual  | [**~AffineBodyPrismaticJoint**](#function-affinebodyprismaticjoint) () <br> |




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
using uipc::constitution::AffineBodyPrismaticJoint::SlotTuple =  std::tuple<S<geometry::SimplicialComplexSlot>, S<geometry::SimplicialComplexSlot> >;
```




<hr>
## Public Functions Documentation




### function AffineBodyPrismaticJoint 

```C++
uipc::constitution::AffineBodyPrismaticJoint::AffineBodyPrismaticJoint (
    const Json & config=default_config()
) 
```




<hr>



### function apply\_to [1/3]

_Deprecated: Apply prismatic joint to edges connecting affine bodies._ 
```C++
void uipc::constitution::AffineBodyPrismaticJoint::apply_to (
    geometry::SimplicialComplex & edges,
    span< SlotTuple > geo_slots,
    Float strength_ratio=Float{100}
) 
```



This method is deprecated. Use the new apply\_to methods with instance IDs for multi-instance support.




**Parameters:**


* `edges` The simplicial complex containing the edges representing the joints. 
* `geo_slots` Pairs of geometry slots representing the connected bodies. 
* `strength_ratio` The strength ratio of the joint constraint (default: 100). 




        

<hr>



### function apply\_to [2/3]

_Apply prismatic joint to edges connecting affine bodies (single-instance mode)._ 
```C++
void uipc::constitution::AffineBodyPrismaticJoint::apply_to (
    geometry::SimplicialComplex & edges,
    span< S< geometry::SimplicialComplexSlot > > l_geo_slots,
    span< S< geometry::SimplicialComplexSlot > > r_geo_slots,
    Float strength_ratio=Float{100}
) 
```



This method assumes each geometry has exactly one instance (instance 0). All joints use the same strength ratio.




**Parameters:**


* `edges` The simplicial complex containing the edges representing the joints. 
* `l_geo_slots` Left geometry slots for each joint. 
* `r_geo_slots` Right geometry slots for each joint. 
* `strength_ratio` The strength ratio of the joint constraint applied to all joints (default: 100). 




        

<hr>



### function apply\_to [3/3]

_Apply prismatic joint to edges connecting affine bodies (multi-instance mode)._ 
```C++
void uipc::constitution::AffineBodyPrismaticJoint::apply_to (
    geometry::SimplicialComplex & edges,
    span< S< geometry::SimplicialComplexSlot > > l_geo_slots,
    span< IndexT > l_instance_id,
    span< S< geometry::SimplicialComplexSlot > > r_geo_slots,
    span< IndexT > r_instance_id,
    span< Float > strength_ratio
) 
```



This method supports geometries with multiple instances. Each joint can specify which instance of each geometry to connect, and can have its own strength ratio.




**Parameters:**


* `edges` The simplicial complex containing the edges representing the joints. 
* `l_geo_slots` Left geometry slots for each joint. 
* `l_instance_id` Instance IDs for the left geometries (must be in range [0, instances().size())). 
* `r_geo_slots` Right geometry slots for each joint. 
* `r_instance_id` Instance IDs for the right geometries (must be in range [0, instances().size())). 
* `strength_ratio` The strength ratio for each joint (one per edge). 




        

<hr>



### function ~AffineBodyPrismaticJoint 

```C++
virtual uipc::constitution::AffineBodyPrismaticJoint::~AffineBodyPrismaticJoint () 
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::AffineBodyPrismaticJoint::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_prismatic_joint.h`

