

# Class uipc::constitution::AffineBodyPrismaticJointExternalForce



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodyPrismaticJointExternalForce**](classuipc_1_1constitution_1_1AffineBodyPrismaticJointExternalForce.md)








Inherits the following classes: [uipc::constitution::Constraint](classuipc_1_1constitution_1_1Constraint.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyPrismaticJointExternalForce**](#function-affinebodyprismaticjointexternalforce) (const Json & config=default\_config()) <br> |
|  void | [**apply\_to**](#function-apply_to-12) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float force=Float{0}) <br>_Apply uniform external force along the prismatic joint axis to all joints._  |
|  void | [**apply\_to**](#function-apply_to-22) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, span&lt; Float &gt; forces) <br>_Apply per-joint external forces along the prismatic joint axis._  |
|   | [**~AffineBodyPrismaticJointExternalForce**](#function-affinebodyprismaticjointexternalforce) () override<br> |


## Public Functions inherited from uipc::constitution::Constraint

See [uipc::constitution::Constraint](classuipc_1_1constitution_1_1Constraint.md)

| Type | Name |
| ---: | :--- |
|   | [**Constraint**](classuipc_1_1constitution_1_1Constraint.md#function-constraint) () noexcept<br> |


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




































































## Protected Functions inherited from uipc::constitution::Constraint

See [uipc::constitution::Constraint](classuipc_1_1constitution_1_1Constraint.md)

| Type | Name |
| ---: | :--- |
|  void | [**apply\_to**](classuipc_1_1constitution_1_1Constraint.md#function-apply_to) ([**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & geo) const<br> |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1Constraint.md#function-get_uid) () noexcept const = 0<br> |


## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid) () noexcept const = 0<br> |








## Public Functions Documentation




### function AffineBodyPrismaticJointExternalForce 

```C++
uipc::constitution::AffineBodyPrismaticJointExternalForce::AffineBodyPrismaticJointExternalForce (
    const Json & config=default_config()
) 
```




<hr>



### function apply\_to [1/2]

_Apply uniform external force along the prismatic joint axis to all joints._ 
```C++
void uipc::constitution::AffineBodyPrismaticJointExternalForce::apply_to (
    geometry::SimplicialComplex & sc,
    Float force=Float{0}
) 
```



Must be applied AFTER [**AffineBodyPrismaticJoint**](classuipc_1_1constitution_1_1AffineBodyPrismaticJoint.md) (constitution\_uid == 20). The force is a scalar: +f\*t applied to body\_i, -f\*t applied to body\_j, where t is the joint tangent direction.




**Parameters:**


* `sc` The simplicial complex containing the edges representing the joints. 
* `force` The scalar force value applied to all joints. 




        

<hr>



### function apply\_to [2/2]

_Apply per-joint external forces along the prismatic joint axis._ 
```C++
void uipc::constitution::AffineBodyPrismaticJointExternalForce::apply_to (
    geometry::SimplicialComplex & sc,
    span< Float > forces
) 
```



Must be applied AFTER [**AffineBodyPrismaticJoint**](classuipc_1_1constitution_1_1AffineBodyPrismaticJoint.md) (constitution\_uid == 20).




**Parameters:**


* `sc` The simplicial complex containing the edges representing the joints. 
* `forces` Per-joint scalar force values (one per edge). 




        

<hr>



### function ~AffineBodyPrismaticJointExternalForce 

```C++
uipc::constitution::AffineBodyPrismaticJointExternalForce::~AffineBodyPrismaticJointExternalForce () override
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::AffineBodyPrismaticJointExternalForce::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_prismatic_joint_external_force.h`

