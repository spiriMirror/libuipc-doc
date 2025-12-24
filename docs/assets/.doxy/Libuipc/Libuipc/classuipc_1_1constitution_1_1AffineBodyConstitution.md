

# Class uipc::constitution::AffineBodyConstitution



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodyConstitution**](classuipc_1_1constitution_1_1AffineBodyConstitution.md)








Inherits the following classes: [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyConstitution**](#function-affinebodyconstitution) (const Json & config=default\_config()) noexcept<br> |
|  void | [**apply\_to**](#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float kappa, Float mass\_density=1e3) const<br> |
|  [**AffineBodyMaterial**](classuipc_1_1constitution_1_1AffineBodyMaterial.md) | [**create\_material**](#function-create_material) (Float kappa) noexcept const<br> |


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
|  Json | [**default\_config**](#function-default_config) () noexcept<br> |












































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](#function-get_uid) () noexcept override const<br> |


## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid) () noexcept const = 0<br> |






## Public Functions Documentation




### function AffineBodyConstitution 

```C++
uipc::constitution::AffineBodyConstitution::AffineBodyConstitution (
    const Json & config=default_config()
) noexcept
```




<hr>



### function apply\_to 

```C++
void uipc::constitution::AffineBodyConstitution::apply_to (
    geometry::SimplicialComplex & sc,
    Float kappa,
    Float mass_density=1e3
) const
```




<hr>



### function create\_material 

```C++
AffineBodyMaterial uipc::constitution::AffineBodyConstitution::create_material (
    Float kappa
) noexcept const
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::AffineBodyConstitution::default_config () noexcept
```




<hr>
## Protected Functions Documentation




### function get\_uid 

```C++
virtual U64 uipc::constitution::AffineBodyConstitution::get_uid () noexcept override const
```



Implements [*uipc::constitution::IConstitution::get\_uid*](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_constitution.h`

