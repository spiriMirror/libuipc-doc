

# Class uipc::constitution::AffineBodyDrivingRevoluteJoint



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodyDrivingRevoluteJoint**](classuipc_1_1constitution_1_1AffineBodyDrivingRevoluteJoint.md)








Inherits the following classes: [uipc::constitution::Constraint](classuipc_1_1constitution_1_1Constraint.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyDrivingRevoluteJoint**](#function-affinebodydrivingrevolutejoint) (const Json & config=default\_config()) <br> |
|  void | [**apply\_to**](#function-apply_to-12) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float strength\_ratio=Float{100}) <br>_Apply driving revolute joint to edges connecting affine bodies (single-instance mode)._  |
|  void | [**apply\_to**](#function-apply_to-22) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, span&lt; Float &gt; strength\_ratios) <br>_Apply driving revolute joint to edges connecting affine bodies (multi-instance mode)._  |
|   | [**~AffineBodyDrivingRevoluteJoint**](#function-affinebodydrivingrevolutejoint) () override<br> |


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




### function AffineBodyDrivingRevoluteJoint 

```C++
uipc::constitution::AffineBodyDrivingRevoluteJoint::AffineBodyDrivingRevoluteJoint (
    const Json & config=default_config()
) 
```




<hr>



### function apply\_to [1/2]

_Apply driving revolute joint to edges connecting affine bodies (single-instance mode)._ 
```C++
void uipc::constitution::AffineBodyDrivingRevoluteJoint::apply_to (
    geometry::SimplicialComplex & sc,
    Float strength_ratio=Float{100}
) 
```



This method assumes each geometry has exactly one instance (instance 0). All joints use the same strength ratio.




**Parameters:**


* `sc` The simplicial complex containing the edges representing the joints. 
* `strength_ratio` The strength ratio of the joint constraint applied to all joints (default: 100). 




        

<hr>



### function apply\_to [2/2]

_Apply driving revolute joint to edges connecting affine bodies (multi-instance mode)._ 
```C++
void uipc::constitution::AffineBodyDrivingRevoluteJoint::apply_to (
    geometry::SimplicialComplex & sc,
    span< Float > strength_ratios
) 
```



This method supports geometries with multiple instances. Each joint can specify which instance of each geometry to connect, and can have its own strength ratio. 

**Parameters:**


* `sc` The simplicial complex containing the edges representing the joints. 
* `strength_ratios` The strength ratio for each joint (one per edge). 




        

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

