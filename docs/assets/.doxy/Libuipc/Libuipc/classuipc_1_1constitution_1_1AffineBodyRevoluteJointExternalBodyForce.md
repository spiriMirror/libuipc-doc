

# Class uipc::constitution::AffineBodyRevoluteJointExternalBodyForce



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodyRevoluteJointExternalBodyForce**](classuipc_1_1constitution_1_1AffineBodyRevoluteJointExternalBodyForce.md)








Inherits the following classes: [uipc::constitution::Constraint](classuipc_1_1constitution_1_1Constraint.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyRevoluteJointExternalBodyForce**](#function-affinebodyrevolutejointexternalbodyforce) (const Json & config=default\_config()) <br> |
|  void | [**apply\_to**](#function-apply_to-12) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float torque=Float{0}) <br>_Apply uniform external torque around the revolute joint axis to all joints._  |
|  void | [**apply\_to**](#function-apply_to-22) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, span&lt; Float &gt; torques) <br>_Apply per-joint external torques around the revolute joint axis._  |
|   | [**~AffineBodyRevoluteJointExternalBodyForce**](#function-affinebodyrevolutejointexternalbodyforce) () override<br> |


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




### function AffineBodyRevoluteJointExternalBodyForce 

```C++
uipc::constitution::AffineBodyRevoluteJointExternalBodyForce::AffineBodyRevoluteJointExternalBodyForce (
    const Json & config=default_config()
) 
```




<hr>



### function apply\_to [1/2]

_Apply uniform external torque around the revolute joint axis to all joints._ 
```C++
void uipc::constitution::AffineBodyRevoluteJointExternalBodyForce::apply_to (
    geometry::SimplicialComplex & sc,
    Float torque=Float{0}
) 
```



Must be applied AFTER [**AffineBodyRevoluteJoint**](classuipc_1_1constitution_1_1AffineBodyRevoluteJoint.md) (constitution\_uid == 18). The torque is a scalar: +τ applied to body\_j, -τ applied to body\_i, where the axis is defined by the edge direction.




**Parameters:**


* `sc` The simplicial complex containing the edges representing the joints. 
* `torque` The scalar torque value applied to all joints. 




        

<hr>



### function apply\_to [2/2]

_Apply per-joint external torques around the revolute joint axis._ 
```C++
void uipc::constitution::AffineBodyRevoluteJointExternalBodyForce::apply_to (
    geometry::SimplicialComplex & sc,
    span< Float > torques
) 
```



Must be applied AFTER [**AffineBodyRevoluteJoint**](classuipc_1_1constitution_1_1AffineBodyRevoluteJoint.md) (constitution\_uid == 18).




**Parameters:**


* `sc` The simplicial complex containing the edges representing the joints. 
* `torques` Per-joint scalar torque values (one per edge). 




        

<hr>



### function ~AffineBodyRevoluteJointExternalBodyForce 

```C++
uipc::constitution::AffineBodyRevoluteJointExternalBodyForce::~AffineBodyRevoluteJointExternalBodyForce () override
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::AffineBodyRevoluteJointExternalBodyForce::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_revolute_joint_external_force.h`

