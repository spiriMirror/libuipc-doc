

# Class uipc::constitution::FiniteElementExternalForce



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**FiniteElementExternalForce**](classuipc_1_1constitution_1_1FiniteElementExternalForce.md)








Inherits the following classes: [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FiniteElementExternalForce**](#function-finiteelementexternalforce) (const Json & config=default\_config()) <br> |
|  void | [**apply\_to**](#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, const Vector3 & force) <br>_Apply external force (3D) to finite element vertices._  |
|   | [**~FiniteElementExternalForce**](#function-finiteelementexternalforce) () <br> |


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




### function FiniteElementExternalForce 

```C++
uipc::constitution::FiniteElementExternalForce::FiniteElementExternalForce (
    const Json & config=default_config()
) 
```




<hr>



### function apply\_to 

_Apply external force (3D) to finite element vertices._ 
```C++
void uipc::constitution::FiniteElementExternalForce::apply_to (
    geometry::SimplicialComplex & sc,
    const Vector3 & force
) 
```





**Parameters:**


* `sc` SimplicialComplex representing finite element geometry 
* `force` 3D force vector applied uniformly to all vertices 




        

<hr>



### function ~FiniteElementExternalForce 

```C++
uipc::constitution::FiniteElementExternalForce::~FiniteElementExternalForce () 
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::FiniteElementExternalForce::default_config () 
```




<hr>
## Protected Functions Documentation




### function get\_uid 

```C++
virtual U64 uipc::constitution::FiniteElementExternalForce::get_uid () noexcept override const
```



Implements [*uipc::constitution::IConstitution::get\_uid*](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/finite_element_external_force.h`

