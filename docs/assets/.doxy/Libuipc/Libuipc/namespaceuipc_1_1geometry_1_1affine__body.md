

# Namespace uipc::geometry::affine\_body



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**affine\_body**](namespaceuipc_1_1geometry_1_1affine__body.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  UIPC\_GEOMETRY\_API Matrix12x12 | [**build\_abd\_mass\_matrix**](#function-build_abd_mass_matrix) (Float m, const Vector3 & m\_x\_bar, const Matrix3x3 & m\_x\_bar\_x\_bar) <br>_Build the 12x12 ABD mass matrix from dyadic mass components._  |
|  UIPC\_GEOMETRY\_API Vector12 | [**compute\_body\_force**](#function-compute_body_force) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, const Vector3 & body\_force\_density) <br>_Compute the body force of an affine body._  |
|  UIPC\_GEOMETRY\_API void | [**compute\_dyadic\_mass**](#function-compute_dyadic_mass) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float rho, Float & m, Vector3 & m\_x\_bar, Matrix3x3 & m\_x\_bar\_x\_bar) <br>_Compute the dyadic mass of a simplicial complex._  |
|  UIPC\_GEOMETRY\_API void | [**compute\_dyadic\_mass**](#function-compute_dyadic_mass) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float rho, Float thickness, Float & m, Vector3 & m\_x\_bar, Matrix3x3 & m\_x\_bar\_x\_bar) <br>_Compute the dyadic mass of a codimensional simplicial complex (shell or rod)._  |
|  UIPC\_GEOMETRY\_API Matrix12x12 | [**from\_rigid\_body**](#function-from_rigid_body) (Float mass, const Vector3 & center\_of\_mass, const Matrix3x3 & inertia\_cm) <br>_Build the 12x12 ABD mass matrix from rigid body quantities._  |
|  Matrix4x4 | [**q\_to\_transform**](#function-q_to_transform) (const Vector12 & q) <br> |
|  Matrix4x4 | [**q\_v\_to\_transform\_v**](#function-q_v_to_transform_v) (const Vector12 & q) <br> |
|  UIPC\_GEOMETRY\_API void | [**to\_rigid\_body**](#function-to_rigid_body) (Float m, const Vector3 & m\_x\_bar, const Matrix3x3 & m\_x\_bar\_x\_bar, Float & total\_mass, Vector3 & center\_of\_mass, Matrix3x3 & inertia\_cm) <br>_Extract rigid body properties from dyadic mass components._  |
|  UIPC\_GEOMETRY\_API void | [**to\_rigid\_body**](#function-to_rigid_body) (const Matrix12x12 & mass\_matrix, Float & total\_mass, Vector3 & center\_of\_mass, Matrix3x3 & inertia\_cm) <br>_Extract rigid body properties from a 12x12 ABD mass matrix._  |
|  Vector12 | [**transform\_to\_q**](#function-transform_to_q) (const Matrix4x4 & trans) <br> |
|  Vector12 | [**transform\_v\_to\_q\_v**](#function-transform_v_to_q_v) (const Matrix4x4 & transform\_v) <br> |




























## Public Functions Documentation




### function build\_abd\_mass\_matrix 

_Build the 12x12 ABD mass matrix from dyadic mass components._ 
```C++
UIPC_GEOMETRY_API Matrix12x12 uipc::geometry::affine_body::build_abd_mass_matrix (
    Float m,
    const Vector3 & m_x_bar,
    const Matrix3x3 & m_x_bar_x_bar
) 
```



Assembles the block-structured mass matrix: M = \| m\*I\_3 I\_3 (x) (mc^T) \| \| I\_3 (x) (mc) I\_3 (x) S \|




**Parameters:**


* `m` Total mass. 
* `m_x_bar` First moment of mass (m \* center\_of\_mass). 
* `m_x_bar_x_bar` Second moment of mass tensor S. 



**Returns:**

The 12x12 ABD mass matrix. 





        

<hr>



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



### function from\_rigid\_body 

_Build the 12x12 ABD mass matrix from rigid body quantities._ 
```C++
UIPC_GEOMETRY_API Matrix12x12 uipc::geometry::affine_body::from_rigid_body (
    Float mass,
    const Vector3 & center_of_mass,
    const Matrix3x3 & inertia_cm
) 
```



Given the standard rigid body properties (mass, center of mass, inertia tensor about the center of mass), this function constructs the equivalent affine body dynamics mass matrix.


Recipe (see scripts/symbol\_calculation/rigid\_body\_to\_affine\_body.ipynb):
* Parallel axis theorem: I^O = I\_cm + m \* (\|c\|^2 I\_3 - c c^T)
* Inertia-to-second-moment inversion: S = 0.5 \* tr(I^O) \* I\_3 - I^O
* Assemble the 12x12 block matrix from (m, m\*c, S).






**Parameters:**


* `mass` Total mass of the rigid body. 
* `center_of_mass` Center of mass in the reference configuration. 
* `inertia_cm` 3x3 inertia tensor about the center of mass. 



**Returns:**

The 12x12 ABD mass matrix. 





        

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



### function to\_rigid\_body 

_Extract rigid body properties from dyadic mass components._ 
```C++
UIPC_GEOMETRY_API void uipc::geometry::affine_body::to_rigid_body (
    Float m,
    const Vector3 & m_x_bar,
    const Matrix3x3 & m_x_bar_x_bar,
    Float & total_mass,
    Vector3 & center_of_mass,
    Matrix3x3 & inertia_cm
) 
```



Inverse of `from_rigid_body`: given the ABD dyadic mass quantities, recovers the total mass, center of mass, and inertia tensor about the center of mass.




**Parameters:**


* `m` Total mass (= sum of element masses). 
* `m_x_bar` First moment of mass (m \* center\_of\_mass). 
* `m_x_bar_x_bar` Second moment of mass tensor S. 
* `total_mass` Total mass (same as m). 
* `center_of_mass` Center of mass in the reference frame. 
* `inertia_cm` 3x3 inertia tensor about the center of mass. 




        

<hr>



### function to\_rigid\_body 

_Extract rigid body properties from a 12x12 ABD mass matrix._ 
```C++
UIPC_GEOMETRY_API void uipc::geometry::affine_body::to_rigid_body (
    const Matrix12x12 & mass_matrix,
    Float & total_mass,
    Vector3 & center_of_mass,
    Matrix3x3 & inertia_cm
) 
```



Convenience overload that decomposes the mass matrix into (m, m\_x\_bar, m\_x\_bar\_x\_bar) and then calls the dyadic-mass version of `to_rigid_body`.




**Parameters:**


* `mass_matrix` The 12x12 ABD mass matrix. 
* `total_mass` Total mass. 
* `center_of_mass` Center of mass in the reference frame. 
* `inertia_cm` 3x3 inertia tensor about the center of mass. 




        

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
The documentation for this class was generated from the following file `include/uipc/geometry/utils/affine_body/affine_body_from_rigid_body.h`

