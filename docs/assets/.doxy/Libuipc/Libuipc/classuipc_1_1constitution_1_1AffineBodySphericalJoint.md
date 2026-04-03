

# Class uipc::constitution::AffineBodySphericalJoint



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodySphericalJoint**](classuipc_1_1constitution_1_1AffineBodySphericalJoint.md)








Inherits the following classes: [uipc::constitution::InterAffineBodyConstitution](classuipc_1_1constitution_1_1InterAffineBodyConstitution.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodySphericalJoint**](#function-affinebodysphericaljoint) (const Json & config=default\_config()) <br> |
|  void | [**apply\_to**](#function-apply_to-12) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; l\_geo\_slots, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; r\_geo\_slots, Float strength\_ratio=Float{100}) <br>_Bind affine body instances to existing spherical joint geometry (single-instance mode)._  |
|  void | [**apply\_to**](#function-apply_to-22) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; l\_geo\_slots, span&lt; IndexT &gt; l\_instance\_ids, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; r\_geo\_slots, span&lt; IndexT &gt; r\_instance\_ids, span&lt; Float &gt; strength\_ratios) <br>_Bind affine body instances to existing spherical joint geometry (multi-instance mode)._  |
|  [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**create\_geometry**](#function-create_geometry-12) (span&lt; const Vector3 &gt; positions, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; l\_geo\_slots, span&lt; IndexT &gt; l\_instance\_ids, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; r\_geo\_slots, span&lt; IndexT &gt; r\_instance\_ids, span&lt; Float &gt; strength\_ratios) <br>_Create spherical joint geometry with world-space anchor positions._  |
|  [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**create\_geometry**](#function-create_geometry-22) (span&lt; const Vector3 &gt; l\_positions, span&lt; const Vector3 &gt; r\_positions, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; l\_geo\_slots, span&lt; IndexT &gt; l\_instance\_ids, span&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; r\_geo\_slots, span&lt; IndexT &gt; r\_instance\_ids, span&lt; Float &gt; strength\_ratios) <br>_Create spherical joint geometry with local-space anchor positions._  |
| virtual  | [**~AffineBodySphericalJoint**](#function-affinebodysphericaljoint) () <br> |




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








## Public Functions Documentation




### function AffineBodySphericalJoint 

```C++
uipc::constitution::AffineBodySphericalJoint::AffineBodySphericalJoint (
    const Json & config=default_config()
) 
```




<hr>



### function apply\_to [1/2]

_Bind affine body instances to existing spherical joint geometry (single-instance mode)._ 
```C++
void uipc::constitution::AffineBodySphericalJoint::apply_to (
    geometry::SimplicialComplex & sc,
    span< S< geometry::SimplicialComplexSlot > > l_geo_slots,
    span< S< geometry::SimplicialComplexSlot > > r_geo_slots,
    Float strength_ratio=Float{100}
) 
```



Pure binding: writes constitution UID, geometry IDs, instance IDs, and strength ratios on vertices. Does NOT build geometry. 


        

<hr>



### function apply\_to [2/2]

_Bind affine body instances to existing spherical joint geometry (multi-instance mode)._ 
```C++
void uipc::constitution::AffineBodySphericalJoint::apply_to (
    geometry::SimplicialComplex & sc,
    span< S< geometry::SimplicialComplexSlot > > l_geo_slots,
    span< IndexT > l_instance_ids,
    span< S< geometry::SimplicialComplexSlot > > r_geo_slots,
    span< IndexT > r_instance_ids,
    span< Float > strength_ratios
) 
```



Pure binding: writes constitution UID, geometry IDs, instance IDs, and strength ratios on vertices. Does NOT build geometry. 


        

<hr>



### function create\_geometry [1/2]

_Create spherical joint geometry with world-space anchor positions._ 
```C++
geometry::SimplicialComplex uipc::constitution::AffineBodySphericalJoint::create_geometry (
    span< const Vector3 > positions,
    span< S< geometry::SimplicialComplexSlot > > l_geo_slots,
    span< IndexT > l_instance_ids,
    span< S< geometry::SimplicialComplexSlot > > r_geo_slots,
    span< IndexT > r_instance_ids,
    span< Float > strength_ratios
) 
```



Builds a vertex-based SimplicialComplex (1 vertex per joint). Writes vertices.position from positions. Does not write local position attributes. 


        

<hr>



### function create\_geometry [2/2]

_Create spherical joint geometry with local-space anchor positions._ 
```C++
geometry::SimplicialComplex uipc::constitution::AffineBodySphericalJoint::create_geometry (
    span< const Vector3 > l_positions,
    span< const Vector3 > r_positions,
    span< S< geometry::SimplicialComplexSlot > > l_geo_slots,
    span< IndexT > l_instance_ids,
    span< S< geometry::SimplicialComplexSlot > > r_geo_slots,
    span< IndexT > r_instance_ids,
    span< Float > strength_ratios
) 
```



Builds a vertex-based SimplicialComplex (1 vertex per joint). Writes local position attributes (l\_position, r\_position) on vertices. 


        

<hr>



### function ~AffineBodySphericalJoint 

```C++
virtual uipc::constitution::AffineBodySphericalJoint::~AffineBodySphericalJoint () 
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::AffineBodySphericalJoint::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_spherical_joint.h`

