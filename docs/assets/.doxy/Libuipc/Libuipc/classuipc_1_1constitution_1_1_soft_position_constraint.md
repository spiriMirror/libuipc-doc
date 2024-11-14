

# Class uipc::constitution::SoftPositionConstraint



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**SoftPositionConstraint**](classuipc_1_1constitution_1_1_soft_position_constraint.md)








Inherits the following classes: [uipc::constitution::Constraint](classuipc_1_1constitution_1_1_constraint.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SoftPositionConstraint**](#function-softpositionconstraint) (const Json & config=default\_config()) noexcept<br> |
|  void | [**apply\_to**](#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc, Float strength\_rate=100.0) const<br>_Apply the constraint to the simplicial complex vertices._  |


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




### function SoftPositionConstraint 

```C++
uipc::constitution::SoftPositionConstraint::SoftPositionConstraint (
    const Json & config=default_config()
) noexcept
```




<hr>



### function apply\_to 

_Apply the constraint to the simplicial complex vertices._ 
```C++
void uipc::constitution::SoftPositionConstraint::apply_to (
    geometry::SimplicialComplex & sc,
    Float strength_rate=100.0
) const
```





**Parameters:**


* `sc` The simplicial complex to apply the constraint to. 
* `strength_rate` The strength of the constraint will be `strength_rate * vertex_mass`. 
* `is_kinematic` If the vertices' kinetic energy is not considered. 




        

<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::SoftPositionConstraint::default_config () 
```




<hr>
## Protected Functions Documentation




### function get\_uid 

```C++
virtual U64 uipc::constitution::SoftPositionConstraint::get_uid () noexcept override const
```



Implements [*uipc::constitution::Constraint::get\_uid*](classuipc_1_1constitution_1_1_constraint.md#function-get_uid)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/soft_position_constraint.h`

