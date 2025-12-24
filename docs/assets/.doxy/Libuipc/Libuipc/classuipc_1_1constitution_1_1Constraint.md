

# Class uipc::constitution::Constraint



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**Constraint**](classuipc_1_1constitution_1_1Constraint.md)








Inherits the following classes: [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)


Inherited by the following classes: [uipc::constitution::AffineBodyDrivingRevoluteJoint](classuipc_1_1constitution_1_1AffineBodyDrivingRevoluteJoint.md),  [uipc::constitution::ExternalArticulationConstraint](classuipc_1_1constitution_1_1ExternalArticulationConstraint.md),  [uipc::constitution::LinearMotor](classuipc_1_1constitution_1_1LinearMotor.md),  [uipc::constitution::RotatingMotor](classuipc_1_1constitution_1_1RotatingMotor.md),  [uipc::constitution::SoftPositionConstraint](classuipc_1_1constitution_1_1SoftPositionConstraint.md),  [uipc::constitution::SoftTransformConstraint](classuipc_1_1constitution_1_1SoftTransformConstraint.md)




















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Constraint**](#function-constraint) () noexcept<br> |


## Public Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**name**](classuipc_1_1constitution_1_1IConstitution.md#function-name) () noexcept const<br> |
|  std::string\_view | [**type**](classuipc_1_1constitution_1_1IConstitution.md#function-type) () noexcept const<br> |
|  U64 | [**uid**](classuipc_1_1constitution_1_1IConstitution.md#function-uid) () noexcept const<br> |
|  const [**builtin::UIDInfo**](structuipc_1_1builtin_1_1UIDInfo.md) & | [**uid\_info**](classuipc_1_1constitution_1_1IConstitution.md#function-uid_info) () noexcept const<br> |
| virtual  | [**~IConstitution**](classuipc_1_1constitution_1_1IConstitution.md#function-iconstitution) () = default<br> |














































## Protected Functions

| Type | Name |
| ---: | :--- |
|  void | [**apply\_to**](#function-apply_to) ([**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & geo) const<br> |
| virtual U64 | [**get\_uid**](#function-get_uid) () noexcept const = 0<br> |


## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid) () noexcept const = 0<br> |






## Public Functions Documentation




### function Constraint 

```C++
uipc::constitution::Constraint::Constraint () noexcept
```




<hr>
## Protected Functions Documentation




### function apply\_to 

```C++
void uipc::constitution::Constraint::apply_to (
    geometry::Geometry & geo
) const
```




<hr>



### function get\_uid 

```C++
virtual U64 uipc::constitution::Constraint::get_uid () noexcept const = 0
```



Implements [*uipc::constitution::IConstitution::get\_uid*](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/constraint.h`

