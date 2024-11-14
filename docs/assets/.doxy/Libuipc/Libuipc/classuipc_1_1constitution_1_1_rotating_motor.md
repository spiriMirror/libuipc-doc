

# Class uipc::constitution::RotatingMotor



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**RotatingMotor**](classuipc_1_1constitution_1_1_rotating_motor.md)








Inherits the following classes: [uipc::constitution::Constraint](classuipc_1_1constitution_1_1_constraint.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**RotatingMotor**](#function-rotatingmotor) (const Json & config=default\_config()) noexcept<br> |
|  void | [**apply\_to**](#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc, Float strength\_ratio=100.0, Vector3 motor\_rot\_axis=Vector3::UnitX(), Float motor\_rot\_vel=2 \*std::numbers::pi) const<br> |


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
|  void | [**animate**](#function-animate) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc, Float dt) <br> |
|  Json | [**default\_config**](#function-default_config) () <br> |


































































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](#function-get_uid) () noexcept override const<br> |


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




### function RotatingMotor 

```C++
uipc::constitution::RotatingMotor::RotatingMotor (
    const Json & config=default_config()
) noexcept
```




<hr>



### function apply\_to 

```C++
void uipc::constitution::RotatingMotor::apply_to (
    geometry::SimplicialComplex & sc,
    Float strength_ratio=100.0,
    Vector3 motor_rot_axis=Vector3::UnitX(),
    Float motor_rot_vel=2 *std::numbers::pi
) const
```




<hr>
## Public Static Functions Documentation




### function animate 

```C++
static void uipc::constitution::RotatingMotor::animate (
    geometry::SimplicialComplex & sc,
    Float dt
) 
```




<hr>



### function default\_config 

```C++
static Json uipc::constitution::RotatingMotor::default_config () 
```




<hr>
## Protected Functions Documentation




### function get\_uid 

```C++
virtual U64 uipc::constitution::RotatingMotor::get_uid () noexcept override const
```



Implements [*uipc::constitution::Constraint::get\_uid*](classuipc_1_1constitution_1_1_constraint.md#function-get_uid)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/soft_transform_constraint.h`

