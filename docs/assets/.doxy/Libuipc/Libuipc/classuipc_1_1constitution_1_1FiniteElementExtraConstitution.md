

# Class uipc::constitution::FiniteElementExtraConstitution



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**FiniteElementExtraConstitution**](classuipc_1_1constitution_1_1FiniteElementExtraConstitution.md)








Inherits the following classes: [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)


Inherited by the following classes: [uipc::constitution::DiscreteShellBending](classuipc_1_1constitution_1_1DiscreteShellBending.md),  [uipc::constitution::KirchhoffRodBending](classuipc_1_1constitution_1_1KirchhoffRodBending.md)






















































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
|  void | [**apply\_to**](#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc) const<br> |
| virtual U64 | [**get\_uid**](#function-get_uid) () noexcept const = 0<br> |


## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid) () noexcept const = 0<br> |






## Protected Functions Documentation




### function apply\_to 

```C++
void uipc::constitution::FiniteElementExtraConstitution::apply_to (
    geometry::SimplicialComplex & sc
) const
```




<hr>



### function get\_uid 

```C++
virtual U64 uipc::constitution::FiniteElementExtraConstitution::get_uid () noexcept const = 0
```



Implements [*uipc::constitution::IConstitution::get\_uid*](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/finite_element_extra_constitution.h`

