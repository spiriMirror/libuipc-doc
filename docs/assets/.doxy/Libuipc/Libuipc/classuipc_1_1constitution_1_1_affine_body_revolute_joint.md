

# Class uipc::constitution::AffineBodyRevoluteJoint



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodyRevoluteJoint**](classuipc_1_1constitution_1_1_affine_body_revolute_joint.md)








Inherits the following classes: [uipc::constitution::InterAffineBodyConstitution](classuipc_1_1constitution_1_1_inter_affine_body_constitution.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::tuple&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1_geometry_slot_t_3_01_simplicial_complex_01_4.md) &gt;, S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1_geometry_slot_t_3_01_simplicial_complex_01_4.md) &gt; &gt; | [**SlotTuple**](#typedef-slottuple)  <br> |




























































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyRevoluteJoint**](#function-affinebodyrevolutejoint) (const Json & config=default\_config()) <br> |
|  void | [**apply\_to**](#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & edges, span&lt; SlotTuple &gt; geo\_slots, Float strength\_ratio=Float{100}) <br> |
| virtual  | [**~AffineBodyRevoluteJoint**](#function-affinebodyrevolutejoint) () <br> |




## Public Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1_i_constitution.md)

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**name**](classuipc_1_1constitution_1_1_i_constitution.md#function-name) () noexcept const<br> |
|  std::string\_view | [**type**](classuipc_1_1constitution_1_1_i_constitution.md#function-type) () noexcept const<br> |
|  U64 | [**uid**](classuipc_1_1constitution_1_1_i_constitution.md#function-uid) () noexcept const<br> |
|  const [**builtin::UIDInfo**](structuipc_1_1builtin_1_1_u_i_d_info.md) & | [**uid\_info**](classuipc_1_1constitution_1_1_i_constitution.md#function-uid_info) () noexcept const<br> |
| virtual  | [**~IConstitution**](classuipc_1_1constitution_1_1_i_constitution.md#function-iconstitution) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Json | [**default\_config**](#function-default_config) () <br> |






































































## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1_i_constitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1_i_constitution.md#function-get_uid) () noexcept const = 0<br> |








## Public Types Documentation




### typedef SlotTuple 

```C++
using uipc::constitution::AffineBodyRevoluteJoint::SlotTuple =  std::tuple<S<geometry::SimplicialComplexSlot>, S<geometry::SimplicialComplexSlot> >;
```




<hr>
## Public Functions Documentation




### function AffineBodyRevoluteJoint 

```C++
uipc::constitution::AffineBodyRevoluteJoint::AffineBodyRevoluteJoint (
    const Json & config=default_config()
) 
```




<hr>



### function apply\_to 

```C++
void uipc::constitution::AffineBodyRevoluteJoint::apply_to (
    geometry::SimplicialComplex & edges,
    span< SlotTuple > geo_slots,
    Float strength_ratio=Float{100}
) 
```




<hr>



### function ~AffineBodyRevoluteJoint 

```C++
virtual uipc::constitution::AffineBodyRevoluteJoint::~AffineBodyRevoluteJoint () 
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::AffineBodyRevoluteJoint::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_revolute_joint.h`

