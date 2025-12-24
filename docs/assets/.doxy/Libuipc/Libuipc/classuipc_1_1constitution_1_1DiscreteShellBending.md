

# Class uipc::constitution::DiscreteShellBending



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**DiscreteShellBending**](classuipc_1_1constitution_1_1DiscreteShellBending.md)








Inherits the following classes: [uipc::constitution::FiniteElementExtraConstitution](classuipc_1_1constitution_1_1FiniteElementExtraConstitution.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DiscreteShellBending**](#function-discreteshellbending) (const Json & json=default\_config()) <br> |
|  void | [**apply\_to**](#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float bending\_stiffness=100.0\_kPa) <br> |




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




































































## Protected Functions inherited from uipc::constitution::FiniteElementExtraConstitution

See [uipc::constitution::FiniteElementExtraConstitution](classuipc_1_1constitution_1_1FiniteElementExtraConstitution.md)

| Type | Name |
| ---: | :--- |
|  void | [**apply\_to**](classuipc_1_1constitution_1_1FiniteElementExtraConstitution.md#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc) const<br> |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1FiniteElementExtraConstitution.md#function-get_uid) () noexcept const = 0<br> |


## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid) () noexcept const = 0<br> |








## Public Functions Documentation




### function DiscreteShellBending 

```C++
uipc::constitution::DiscreteShellBending::DiscreteShellBending (
    const Json & json=default_config()
) 
```




<hr>



### function apply\_to 

```C++
void uipc::constitution::DiscreteShellBending::apply_to (
    geometry::SimplicialComplex & sc,
    Float bending_stiffness=100.0_kPa
) 
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::DiscreteShellBending::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/discrete_shell_bending.h`

