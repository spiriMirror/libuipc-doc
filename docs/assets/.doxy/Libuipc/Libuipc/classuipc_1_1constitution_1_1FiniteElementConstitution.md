

# Class uipc::constitution::FiniteElementConstitution



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**FiniteElementConstitution**](classuipc_1_1constitution_1_1FiniteElementConstitution.md)








Inherits the following classes: [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)


Inherited by the following classes: [uipc::constitution::ARAP](classuipc_1_1constitution_1_1ARAP.md),  [uipc::constitution::Empty](classuipc_1_1constitution_1_1Empty.md),  [uipc::constitution::HookeanSpring](classuipc_1_1constitution_1_1HookeanSpring.md),  [uipc::constitution::NeoHookeanShell](classuipc_1_1constitution_1_1NeoHookeanShell.md),  [uipc::constitution::Particle](classuipc_1_1constitution_1_1Particle.md),  [uipc::constitution::StableNeoHookean](classuipc_1_1constitution_1_1StableNeoHookean.md),  [uipc::constitution::StrainLimitingBaraffWitkinShell](classuipc_1_1constitution_1_1StrainLimitingBaraffWitkinShell.md)






















































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
|  void | [**apply\_to**](#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float mass\_density, Float thickness=0.0) const<br> |


## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid) () noexcept const = 0<br> |






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

