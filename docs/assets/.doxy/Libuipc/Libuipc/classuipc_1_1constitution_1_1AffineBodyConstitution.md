

# Class uipc::constitution::AffineBodyConstitution



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodyConstitution**](classuipc_1_1constitution_1_1AffineBodyConstitution.md)








Inherits the following classes: [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)


Inherited by the following classes: [uipc::constitution::AffineBodyRod](classuipc_1_1constitution_1_1AffineBodyRod.md),  [uipc::constitution::AffineBodyShell](classuipc_1_1constitution_1_1AffineBodyShell.md)




















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyConstitution**](#function-affinebodyconstitution) (const Json & config=default\_config()) noexcept<br> |
|  void | [**apply\_to**](#function-apply_to-12) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float kappa, Float mass\_density=1e3) const<br> |
|  void | [**apply\_to**](#function-apply_to-22) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float kappa, const Matrix12x12 & mass, Float volume) const<br>_Apply ABD constitution with explicit mass matrix and volume override._  |
|  [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**create\_proxy**](#function-create_proxy-12) (Float kappa, Float mass, const Vector3 & mass\_center, const Matrix3x3 & inertia, Float volume) const<br>_Create a 1-vertex proxy affine body from rigid body mass properties._  |
|  [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**create\_proxy**](#function-create_proxy-22) (Float kappa, const Matrix12x12 & abd\_mass, Float volume) const<br>_Create a 1-vertex proxy affine body from a precomputed 12x12 ABD mass matrix._  |


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
|  void | [**create\_attributes**](#function-create_attributes) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float kappa, Float mass\_density, Float volume, Float m, const Vector3 & m\_x\_bar, const Matrix3x3 & m\_x\_bar\_x\_bar) const<br>_Common ABD attribute setup._  |
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



### function apply\_to [1/2]

```C++
void uipc::constitution::AffineBodyConstitution::apply_to (
    geometry::SimplicialComplex & sc,
    Float kappa,
    Float mass_density=1e3
) const
```




<hr>



### function apply\_to [2/2]

_Apply ABD constitution with explicit mass matrix and volume override._ 
```C++
void uipc::constitution::AffineBodyConstitution::apply_to (
    geometry::SimplicialComplex & sc,
    Float kappa,
    const Matrix12x12 & mass,
    Float volume
) const
```



The 12x12 mass matrix is decomposed into (m, m\_x\_bar, m\_x\_bar\_x\_bar) and stored as meta attributes so the backend uses them directly instead of computing from mesh geometry. 


        

<hr>



### function create\_proxy [1/2]

_Create a 1-vertex proxy affine body from rigid body mass properties._ 
```C++
geometry::SimplicialComplex uipc::constitution::AffineBodyConstitution::create_proxy (
    Float kappa,
    Float mass,
    const Vector3 & mass_center,
    const Matrix3x3 & inertia,
    Float volume
) const
```



The returned SimplicialComplex has a single vertex at the origin and carries all ABD meta attributes. It participates in dynamics (gravity, shape energy) but has no collision geometry. 


        

<hr>



### function create\_proxy [2/2]

_Create a 1-vertex proxy affine body from a precomputed 12x12 ABD mass matrix._ 
```C++
geometry::SimplicialComplex uipc::constitution::AffineBodyConstitution::create_proxy (
    Float kappa,
    const Matrix12x12 & abd_mass,
    Float volume
) const
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::AffineBodyConstitution::default_config () noexcept
```




<hr>
## Protected Functions Documentation




### function create\_attributes 

_Common ABD attribute setup._ 
```C++
void uipc::constitution::AffineBodyConstitution::create_attributes (
    geometry::SimplicialComplex & sc,
    Float kappa,
    Float mass_density,
    Float volume,
    Float m,
    const Vector3 & m_x_bar,
    const Matrix3x3 & m_x_bar_x_bar
) const
```



Sets constitution\_uid, transforms, dof\_offset, dof\_count, is\_fixed, is\_dynamic, external\_kinetic, velocity, self\_collision, kappa, volume, mass\_density, abd\_mass/abd\_mass\_x\_bar/abd\_mass\_x\_bar\_x\_bar, and user-facing mass/mass\_center/inertia on sc.meta().


Subclasses ([**AffineBodyShell**](classuipc_1_1constitution_1_1AffineBodyShell.md), [**AffineBodyRod**](classuipc_1_1constitution_1_1AffineBodyRod.md)) call this with their own pre-computed volume and dyadic mass. 


        

<hr>



### function get\_uid 

```C++
virtual U64 uipc::constitution::AffineBodyConstitution::get_uid () noexcept override const
```



Implements [*uipc::constitution::IConstitution::get\_uid*](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_constitution.h`

