

# Class uipc::constitution::ExternalArticulationConstraint



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**ExternalArticulationConstraint**](classuipc_1_1constitution_1_1ExternalArticulationConstraint.md)



_External articulation constraint for incorporating external kinetic energy into the IPC system._ [More...](#detailed-description)

* `#include <external_articulation_constraint.h>`



Inherits the following classes: [uipc::constitution::Constraint](classuipc_1_1constitution_1_1Constraint.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ExternalArticulationConstraint**](#function-externalarticulationconstraint) (const Json & config=[**default\_config**](classuipc_1_1constitution_1_1ExternalArticulationConstraint.md#function-default_config)()) noexcept<br>_Construct an_ [_**ExternalArticulationConstraint**_](classuipc_1_1constitution_1_1ExternalArticulationConstraint.md) _._ |
|  [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) | [**create\_geometry**](#function-create_geometry-12) (span&lt; S&lt; const [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &gt; &gt; joint\_geos) const<br>_Create geometry for external articulation joints._  |
|  [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) | [**create\_geometry**](#function-create_geometry-22) (span&lt; S&lt; const [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &gt; &gt; joint\_geos, span&lt; IndexT &gt; indices) const<br>_Create geometry for external articulation joints with specified indices._  |
|   | [**~ExternalArticulationConstraint**](#function-externalarticulationconstraint) () <br>_Destructor._  |


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
|  Json | [**default\_config**](#function-default_config) () <br>_Get the default configuration for_ [_**ExternalArticulationConstraint**_](classuipc_1_1constitution_1_1ExternalArticulationConstraint.md) _._ |


































































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](#function-get_uid) () noexcept override const<br>_Get the unique identifier for this constraint type._  |


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








## Detailed Description


Controls motion of affine bodies by prescribing articulation DOFs (joint positions, angles, etc.). Incorporates kinetic energy term: K = 1/2(delta\_theta - delta\_theta\_tilde)^T M^t (delta\_theta - delta\_theta\_tilde) where delta\_theta is variational joint DOF, delta\_theta\_tilde is predicted variational joint DOF, and M^t is effective mass matrix at previous time step.


Users must provide M^t and delta\_theta\_tilde through animator callback. Works with [**AffineBodyRevoluteJoint**](classuipc_1_1constitution_1_1AffineBodyRevoluteJoint.md) and [**AffineBodyPrismaticJoint**](classuipc_1_1constitution_1_1AffineBodyPrismaticJoint.md) to constrain affine bodies to follow articulation motion. 


    
## Public Functions Documentation




### function ExternalArticulationConstraint 

_Construct an_ [_**ExternalArticulationConstraint**_](classuipc_1_1constitution_1_1ExternalArticulationConstraint.md) _._
```C++
uipc::constitution::ExternalArticulationConstraint::ExternalArticulationConstraint (
    const Json & config=default_config ()
) noexcept
```





**Parameters:**


* `config` Configuration dictionary (optional, uses default if not provided). 




        

<hr>



### function create\_geometry [1/2]

_Create geometry for external articulation joints._ 
```C++
geometry::Geometry uipc::constitution::ExternalArticulationConstraint::create_geometry (
    span< S< const geometry::GeometrySlot > > joint_geos
) const
```



Creates geometry structure with joint attributes (geo\_id, index, delta\_theta\_tilde, delta\_theta) and joint-joint mass attributes. All joints use index 0 by default.




**Parameters:**


* `joint_geos` Geometry slots containing joint information. 



**Returns:**

[**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) Created geometry with joint constraint data. 





        

<hr>



### function create\_geometry [2/2]

_Create geometry for external articulation joints with specified indices._ 
```C++
geometry::Geometry uipc::constitution::ExternalArticulationConstraint::create_geometry (
    span< S< const geometry::GeometrySlot > > joint_geos,
    span< IndexT > indices
) const
```



Same as single-parameter version but allows selecting specific joints from each geometry slot.




**Parameters:**


* `joint_geos` Geometry slots containing joint information. 
* `indices` Indices specifying which joint to use from each slot. Must match joint\_geos size. 



**Returns:**

[**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) Created geometry with joint constraint data. 





        

<hr>



### function ~ExternalArticulationConstraint 

_Destructor._ 
```C++
uipc::constitution::ExternalArticulationConstraint::~ExternalArticulationConstraint () 
```




<hr>
## Public Static Functions Documentation




### function default\_config 

_Get the default configuration for_ [_**ExternalArticulationConstraint**_](classuipc_1_1constitution_1_1ExternalArticulationConstraint.md) _._
```C++
static Json uipc::constitution::ExternalArticulationConstraint::default_config () 
```





**Returns:**

Json Default configuration dictionary (currently empty). 





        

<hr>
## Protected Functions Documentation




### function get\_uid 

_Get the unique identifier for this constraint type._ 
```C++
virtual U64 uipc::constitution::ExternalArticulationConstraint::get_uid () noexcept override const
```





**Returns:**

U64 The constraint UID. 





        
Implements [*uipc::constitution::Constraint::get\_uid*](classuipc_1_1constitution_1_1Constraint.md#function-get_uid)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/external_articulation_constraint.h`

