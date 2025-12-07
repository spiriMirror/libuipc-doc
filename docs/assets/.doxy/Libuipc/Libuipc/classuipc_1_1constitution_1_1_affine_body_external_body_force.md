

# Class uipc::constitution::AffineBodyExternalBodyForce



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodyExternalBodyForce**](classuipc_1_1constitution_1_1_affine_body_external_body_force.md)








Inherits the following classes: [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1_i_constitution.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyExternalBodyForce**](#function-affinebodyexternalbodyforce) (const Json & config=default\_config()) <br> |
|  void | [**apply\_to**](#function-apply_to-12) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc, const Vector12 & force) <br>_Apply external force (12D generalized force) to affine body instances._  |
|  void | [**apply\_to**](#function-apply_to-22) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc, const Vector3 & force) <br>_Apply external translational force to affine body instances (only translational force, affine force = 0)_  |
|   | [**~AffineBodyExternalBodyForce**](#function-affinebodyexternalbodyforce) () <br> |


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


## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1_i_constitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1_i_constitution.md#function-get_uid) () noexcept const = 0<br> |






## Public Functions Documentation




### function AffineBodyExternalBodyForce 

```C++
uipc::constitution::AffineBodyExternalBodyForce::AffineBodyExternalBodyForce (
    const Json & config=default_config()
) 
```




<hr>



### function apply\_to [1/2]

_Apply external force (12D generalized force) to affine body instances._ 
```C++
void uipc::constitution::AffineBodyExternalBodyForce::apply_to (
    geometry::SimplicialComplex & sc,
    const Vector12 & force
) 
```





**Parameters:**


* `sc` SimplicialComplex representing affine body geometry 
* `force` 12D generalized force vector: [fx, fy, fz, f\_a11, f\_a12, f\_a13, f\_a21, f\_a22, f\_a23, f\_a31, f\_a32, f\_a33] where f is the 3D translational force and f\_a is the 9D affine force 




        

<hr>



### function apply\_to [2/2]

_Apply external translational force to affine body instances (only translational force, affine force = 0)_ 
```C++
void uipc::constitution::AffineBodyExternalBodyForce::apply_to (
    geometry::SimplicialComplex & sc,
    const Vector3 & force
) 
```





**Parameters:**


* `sc` SimplicialComplex representing affine body geometry 
* `force` 3D translational force vector 




        

<hr>



### function ~AffineBodyExternalBodyForce 

```C++
uipc::constitution::AffineBodyExternalBodyForce::~AffineBodyExternalBodyForce () 
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::AffineBodyExternalBodyForce::default_config () 
```




<hr>
## Protected Functions Documentation




### function get\_uid 

```C++
virtual U64 uipc::constitution::AffineBodyExternalBodyForce::get_uid () noexcept override const
```



Implements [*uipc::constitution::IConstitution::get\_uid*](classuipc_1_1constitution_1_1_i_constitution.md#function-get_uid)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_external_force.h`

