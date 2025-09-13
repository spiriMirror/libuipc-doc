

# Class uipc::constitution::AffineBodyDrivingRevoluteJoint



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodyDrivingRevoluteJoint**](classuipc_1_1constitution_1_1_affine_body_driving_revolute_joint.md)








Inherits the following classes: [uipc::constitution::Constraint](classuipc_1_1constitution_1_1_constraint.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyDrivingRevoluteJoint**](#function-affinebodydrivingrevolutejoint) (const Json & config=default\_config()) <br> |
|  void | [**apply\_to**](#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc, Float strength\_ratio=Float{100}) <br> |
|   | [**~AffineBodyDrivingRevoluteJoint**](#function-affinebodydrivingrevolutejoint) () override<br> |


## Public Functions inherited from uipc::constitution::Constraint

See [uipc::constitution::Constraint](classuipc_1_1constitution_1_1_constraint.md)

| Type | Name |
| ---: | :--- |
|   | [**Constraint**](classuipc_1_1constitution_1_1_constraint.md#function-constraint) () noexcept<br> |


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




































































## Protected Functions inherited from uipc::constitution::Constraint

See [uipc::constitution::Constraint](classuipc_1_1constitution_1_1_constraint.md)

| Type | Name |
| ---: | :--- |
|  void | [**apply\_to**](classuipc_1_1constitution_1_1_constraint.md#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc) const<br> |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1_constraint.md#function-get_uid) () noexcept const = 0<br> |


## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1_i_constitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1_i_constitution.md#function-get_uid) () noexcept const = 0<br> |








## Public Functions Documentation




### function AffineBodyDrivingRevoluteJoint 

```C++
uipc::constitution::AffineBodyDrivingRevoluteJoint::AffineBodyDrivingRevoluteJoint (
    const Json & config=default_config()
) 
```




<hr>



### function apply\_to 

```C++
void uipc::constitution::AffineBodyDrivingRevoluteJoint::apply_to (
    geometry::SimplicialComplex & sc,
    Float strength_ratio=Float{100}
) 
```




<hr>



### function ~AffineBodyDrivingRevoluteJoint 

```C++
uipc::constitution::AffineBodyDrivingRevoluteJoint::~AffineBodyDrivingRevoluteJoint () override
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::AffineBodyDrivingRevoluteJoint::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_driving_revolute_joint.h`

