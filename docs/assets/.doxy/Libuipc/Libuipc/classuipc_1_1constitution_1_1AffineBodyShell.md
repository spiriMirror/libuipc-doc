

# Class uipc::constitution::AffineBodyShell



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodyShell**](classuipc_1_1constitution_1_1AffineBodyShell.md)



_Codimensional 2D (shell) affine body constitution._ [More...](#detailed-description)

* `#include <affine_body_shell.h>`



Inherits the following classes: [uipc::constitution::AffineBodyConstitution](classuipc_1_1constitution_1_1AffineBodyConstitution.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyShell**](#function-affinebodyshell) (const Json & config=default\_config()) noexcept<br> |
|  void | [**apply\_to**](#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float kappa, Float mass\_density=1e3, Float thickness=0.01) const<br>_Apply the shell constitution to a 2D simplicial complex._  |


## Public Functions inherited from uipc::constitution::AffineBodyConstitution

See [uipc::constitution::AffineBodyConstitution](classuipc_1_1constitution_1_1AffineBodyConstitution.md)

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyConstitution**](classuipc_1_1constitution_1_1AffineBodyConstitution.md#function-affinebodyconstitution) (const Json & config=default\_config()) noexcept<br> |
|  void | [**apply\_to**](classuipc_1_1constitution_1_1AffineBodyConstitution.md#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float kappa, Float mass\_density=1e3) const<br> |
|  [**AffineBodyMaterial**](classuipc_1_1constitution_1_1AffineBodyMaterial.md) | [**create\_material**](classuipc_1_1constitution_1_1AffineBodyConstitution.md#function-create_material) (Float kappa) noexcept const<br> |


## Public Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**name**](classuipc_1_1constitution_1_1IConstitution.md#function-name) () noexcept const<br> |
|  std::string\_view | [**type**](classuipc_1_1constitution_1_1IConstitution.md#function-type) () noexcept const<br> |
|  U64 | [**uid**](classuipc_1_1constitution_1_1IConstitution.md#function-uid) () noexcept const<br> |
|  const [**builtin::UIDInfo**](structuipc_1_1builtin_1_1UIDInfo.md) & | [**uid\_info**](classuipc_1_1constitution_1_1IConstitution.md#function-uid_info) () noexcept const<br> |
| virtual  | [**~IConstitution**](classuipc_1_1constitution_1_1IConstitution.md#function-iconstitution) () = default<br> |




## Public Static Functions inherited from uipc::constitution::AffineBodyConstitution

See [uipc::constitution::AffineBodyConstitution](classuipc_1_1constitution_1_1AffineBodyConstitution.md)

| Type | Name |
| ---: | :--- |
|  Json | [**default\_config**](classuipc_1_1constitution_1_1AffineBodyConstitution.md#function-default_config) () noexcept<br> |


































































## Protected Functions inherited from uipc::constitution::AffineBodyConstitution

See [uipc::constitution::AffineBodyConstitution](classuipc_1_1constitution_1_1AffineBodyConstitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1AffineBodyConstitution.md#function-get_uid) () noexcept override const<br> |
|  void | [**setup\_abd\_attributes**](classuipc_1_1constitution_1_1AffineBodyConstitution.md#function-setup_abd_attributes) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float kappa, Float mass\_density, Float volume) const<br>_Common ABD attribute setup without volume computation._  |


## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid) () noexcept const = 0<br> |








## Detailed Description


Convenience subclass of [**AffineBodyConstitution**](classuipc_1_1constitution_1_1AffineBodyConstitution.md) for open triangle meshes treated as thin shells with a given thickness.


Uses the same UID as [**AffineBodyConstitution**](classuipc_1_1constitution_1_1AffineBodyConstitution.md) (OrthoPotential = 1 by default). Sets `builtin::is_codim = 1` on the geometry meta so the backend uses the codim dyadic mass computation path. 


    
## Public Functions Documentation




### function AffineBodyShell 

```C++
uipc::constitution::AffineBodyShell::AffineBodyShell (
    const Json & config=default_config()
) noexcept
```




<hr>



### function apply\_to 

_Apply the shell constitution to a 2D simplicial complex._ 
```C++
void uipc::constitution::AffineBodyShell::apply_to (
    geometry::SimplicialComplex & sc,
    Float kappa,
    Float mass_density=1e3,
    Float thickness=0.01
) const
```





**Parameters:**


* `sc` The triangle mesh (dim == 2). 
* `kappa` Stiffness parameter for shape energy. 
* `mass_density` Volume mass density (kg/m³). 
* `thickness` Shell thickness radius `r` (effective slab thickness = 2r). 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_shell.h`

