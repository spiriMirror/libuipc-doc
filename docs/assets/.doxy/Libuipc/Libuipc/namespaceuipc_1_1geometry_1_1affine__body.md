

# Namespace uipc::geometry::affine\_body



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**affine\_body**](namespaceuipc_1_1geometry_1_1affine__body.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  UIPC\_GEOMETRY\_API Vector12 | [**compute\_body\_force**](#function-compute_body_force) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc, const Vector3 & body\_force\_density) <br>_Compute the body force of an affine body._  |
|  UIPC\_GEOMETRY\_API void | [**compute\_dyadic\_mass**](#function-compute_dyadic_mass) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc, Float rho, Float & m, Vector3 & m\_x\_bar, Matrix3x3 & m\_x\_bar\_x\_bar) <br>_Compute the dyadic mass of a simplicial complex._  |




























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
* `body_force` The body force 




        

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

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/utils/affine_body/compute_body_force.h`

