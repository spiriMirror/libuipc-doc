

# Class uipc::constitution::FiniteElementConstitution



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**FiniteElementConstitution**](classuipc_1_1constitution_1_1_finite_element_constitution.md)








Inherits the following classes: [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1_i_constitution.md)


Inherited by the following classes: [uipc::constitution::ARAP](classuipc_1_1constitution_1_1_a_r_a_p.md),  [uipc::constitution::Empty](classuipc_1_1constitution_1_1_empty.md),  [uipc::constitution::HookeanSpring](classuipc_1_1constitution_1_1_hookean_spring.md),  [uipc::constitution::NeoHookeanShell](classuipc_1_1constitution_1_1_neo_hookean_shell.md),  [uipc::constitution::Particle](classuipc_1_1constitution_1_1_particle.md),  [uipc::constitution::StableNeoHookean](classuipc_1_1constitution_1_1_stable_neo_hookean.md),  [uipc::constitution::StrainLimitingBaraffWitkinShell](classuipc_1_1constitution_1_1_strain_limiting_baraff_witkin_shell.md)






















































## Public Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1_i_constitution.md)

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**name**](classuipc_1_1constitution_1_1_i_constitution.md#function-name) () noexcept const<br> |
|  std::string\_view | [**type**](classuipc_1_1constitution_1_1_i_constitution.md#function-type) () noexcept const<br> |
|  U64 | [**uid**](classuipc_1_1constitution_1_1_i_constitution.md#function-uid) () noexcept const<br> |
|  const [**builtin::UIDInfo**](structuipc_1_1builtin_1_1_u_i_d_info.md) & | [**uid\_info**](classuipc_1_1constitution_1_1_i_constitution.md#function-uid_info) () noexcept const<br> |
| virtual  | [**~IConstitution**](classuipc_1_1constitution_1_1_i_constitution.md#function-iconstitution) () = default<br> |














































## Protected Functions

| Type | Name |
| ---: | :--- |
|  void | [**apply\_to**](#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc, Float mass\_density, Float thickness=0.0) const<br> |


## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1_i_constitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1_i_constitution.md#function-get_uid) () noexcept const = 0<br> |






## Protected Functions Documentation




### function apply\_to 

```C++
void uipc::constitution::FiniteElementConstitution::apply_to (
    geometry::SimplicialComplex & sc,
    Float mass_density,
    Float thickness=0.0
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/finite_element_constitution.h`

