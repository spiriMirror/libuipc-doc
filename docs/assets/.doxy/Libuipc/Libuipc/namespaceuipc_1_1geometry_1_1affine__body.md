

# Namespace uipc::geometry::affine\_body



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**affine\_body**](namespaceuipc_1_1geometry_1_1affine__body.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  UIPC\_GEOMETRY\_API Vector12 | [**compute\_body\_force**](#function-compute_body_force) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, const Vector3 & body\_force\_density) <br>_Compute the body force of an affine body._  |
|  UIPC\_GEOMETRY\_API void | [**compute\_dyadic\_mass**](#function-compute_dyadic_mass) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float rho, Float & m, Vector3 & m\_x\_bar, Matrix3x3 & m\_x\_bar\_x\_bar) <br>_Compute the dyadic mass of a simplicial complex._  |
|  UIPC\_GEOMETRY\_API void | [**compute\_dyadic\_mass**](#function-compute_dyadic_mass) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float rho, Float thickness, Float & m, Vector3 & m\_x\_bar, Matrix3x3 & m\_x\_bar\_x\_bar) <br>_Compute the dyadic mass of a codimensional simplicial complex (shell or rod)._  |
|  Matrix4x4 | [**q\_to\_transform**](#function-q_to_transform) (const Vector12 & q) <br> |
|  Matrix4x4 | [**q\_v\_to\_transform\_v**](#function-q_v_to_transform_v) (const Vector12 & q) <br> |
|  Vector12 | [**transform\_to\_q**](#function-transform_to_q) (const Matrix4x4 & trans) <br> |
|  Vector12 | [**transform\_v\_to\_q\_v**](#function-transform_v_to_q_v) (const Matrix4x4 & transform\_v) <br> |




























## Public Functions Documentation




### function compute\_body\_force 

_Compute the body force of an affine body._ 
```C++
UIPC_GEOMETRY_API Vector12 uipc::geometry::affine_body::compute_body_force (
    const SimplicialComplex & sc,
    const Vector3 & body_force_density
) 
```





**Parameters:**


* `sc` The simplicial complex. 
* `body_force_density` The body force density in N/m^3. 




        

<hr>



### function compute\_dyadic\_mass 

_Compute the dyadic mass of a simplicial complex._ 
```C++
UIPC_GEOMETRY_API void uipc::geometry::affine_body::compute_dyadic_mass (
    const SimplicialComplex & sc,
    Float rho,
    Float & m,
    Vector3 & m_x_bar,
    Matrix3x3 & m_x_bar_x_bar
) 
```



Integrate the mass density over the simplicial complex to compute the dyadic mass.




**Parameters:**


* `sc` The simplicial complex.
* `m` The total mass.
* `m_x_bar` The total mass times the center of mass.
* `m_x_bar_x_bar` The total mass times the center of mass times the center of mass transpose. 




        

<hr>



### function compute\_dyadic\_mass 

_Compute the dyadic mass of a codimensional simplicial complex (shell or rod)._ 
```C++
UIPC_GEOMETRY_API void uipc::geometry::affine_body::compute_dyadic_mass (
    const SimplicialComplex & sc,
    Float rho,
    Float thickness,
    Float & m,
    Vector3 & m_x_bar,
    Matrix3x3 & m_x_bar_x_bar
) 
```



Integrates the mass density over the effective 3D volume of the codim body, accounting for thickness to produce an invertible 12×12 ABD mass matrix.



* dim==2 (shell): direct area integration × 2r, plus normal-direction correction.
* dim==1 (rod): segment integration × π r², plus cross-section correction.






**Parameters:**


* `sc` The simplicial complex (triangle mesh for shell, edge mesh for rod). 
* `rho` Volume mass density (kg/m³). 
* `thickness` Thickness radius `r` (half-thickness for shell, cross-section radius for rod). 
* `m` The total mass. 
* `m_x_bar` The total mass times the center of mass. 
* `m_x_bar_x_bar` The second dyadic moment (including thickness correction). 




        

<hr>



### function q\_to\_transform 

```C++
inline Matrix4x4 uipc::geometry::affine_body::q_to_transform (
    const Vector12 & q
) 
```




<hr>



### function q\_v\_to\_transform\_v 

```C++
inline Matrix4x4 uipc::geometry::affine_body::q_v_to_transform_v (
    const Vector12 & q
) 
```




<hr>



### function transform\_to\_q 

```C++
inline Vector12 uipc::geometry::affine_body::transform_to_q (
    const Matrix4x4 & trans
) 
```




<hr>



### function transform\_v\_to\_q\_v 

```C++
inline Vector12 uipc::geometry::affine_body::transform_v_to_q_v (
    const Matrix4x4 & transform_v
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/utils/affine_body/compute_body_force.h`

