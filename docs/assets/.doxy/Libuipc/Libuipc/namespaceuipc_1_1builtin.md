

# Namespace uipc::builtin



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**builtin**](namespaceuipc_1_1builtin.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**details**](namespaceuipc_1_1builtin_1_1details.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**ConstitutionUIDAutoRegister**](classuipc_1_1builtin_1_1_constitution_u_i_d_auto_register.md) <br> |
| class | [**ConstitutionUIDCollection**](classuipc_1_1builtin_1_1_constitution_u_i_d_collection.md) <br> |
| class | [**ImplicitGeometryUIDAutoRegister**](classuipc_1_1builtin_1_1_implicit_geometry_u_i_d_auto_register.md) <br> |
| class | [**ImplicitGeometryUIDCollection**](classuipc_1_1builtin_1_1_implicit_geometry_u_i_d_collection.md) <br> |
| struct | [**UIDInfo**](structuipc_1_1builtin_1_1_u_i_d_info.md) <br> |






## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**AbstractSimplicialComplex**](#variable-abstractsimplicialcomplex)   = `"AbstractSimplicialComplex"`<br> |
|  std::string\_view | [**AffineBody**](#variable-affinebody)   = `"AffineBody"`<br> |
|  std::string\_view | [**Constraint**](#variable-constraint)   = `"Constraint"`<br> |
|  std::string\_view | [**FiniteElement**](#variable-finiteelement)   = `"FiniteElement"`<br> |
|  std::string\_view | [**Geometry**](#variable-geometry)   = `"Geometry"`<br> |
|  std::string\_view | [**ImplicitGeometry**](#variable-implicitgeometry)   = `"ImplicitGeometry"`<br> |
|  std::string\_view | [**InterAffineBody**](#variable-interaffinebody)   = `"InterAffineBody"`<br> |
|  std::string\_view | [**SimplicialComplex**](#variable-simplicialcomplex)   = `"SimplicialComplex"`<br> |
|  std::string\_view | [**\_\_data\_\_**](#variable-__data__)   = `"\_\_data\_\_"`<br> |
|  std::string\_view | [**\_\_meta\_\_**](#variable-__meta__)   = `"\_\_meta\_\_"`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (topo) <br>`topo` _attribute on_**vertices** _/_**edges** _/_**triangles** _/_**tetrahedra** _... to indicate the topological type of the element._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (position) <br>`position` _&lt;Vector3&gt; attribute on_**vertices** __ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (velocity) <br>`velocity` _&lt;Vector3&gt; attribute on_**vertices** _or_`velocity` _&lt;Matrix4x4&gt; attribute on_**instances** _(the derivative of the transform matrix)._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (aim\_position) <br>`aim_position` _&lt;Vector3&gt; attribute on_**vertices** _, indicates the aim position of the vertices if the vertices are animated._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (transform) <br>`transform` _&lt;Matrix4x4&gt; attribute on_**instances** __ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (aim\_transform) <br>`aim_transform` _&lt;Matrix4x4&gt; attribute on_**instances** _, indicates the aim transform of the instances if the instances are animated._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (contact\_element\_id) <br>`contact_element_id` _&lt;IndexT&gt; attribute on_**meta** __ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (constitution\_uid) <br>`constitution_uid` _&lt;U64&gt; attribute on_**meta** _, uid is a unique identifier for a constitution which is defined in the libuipc specification._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (extra\_constitution\_uids) <br>`extra_constitution_uids` _&lt;VectorXu64&gt; attribute on_**meta** _, extra constitutions that are applied to the geometry._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (constraint\_uid) <br>`constraint_uid` _&lt;U64&gt; attribute on_**meta** _, uid is a unique identifier for a constraint which is defined in the libuipc specification._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (implicit\_geometry\_uid) <br>`implicit_geometry_uid` _&lt;U64&gt; attribute on_**meta** _, uid is a unique identifier for an implicit geometry which is defined in the libuipc specification._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (is\_surf) <br>`is_surf` _&lt;IndexT&gt; attribute on_**vertices** _/_**edges** _/_**triangles** _/_**tetrahedra** _... to indicate if the element is a surface element._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (is\_facet) <br>`is_facet` _&lt;IndexT&gt; attribute on_**vertices** _/_**edges** _/_**triangles** _/_**tetrahedra** _to indicate if the element is a facet element._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (orient) <br>`orient` _&lt;IndexT&gt;[-1,0,1] attribute on_**triangles** _to indicate the orientation of the triangle._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (parent\_id) <br>`parent_id` _&lt;IndexT&gt; attribute on_**edges** _/_**triangles** _, indicates the parent simplex id_ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (is\_fixed) <br>`is_fixed` _&lt;IndexT&gt;[0,1] attribute, indicates if the_**instance** _or_**vertex** _is fixed._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (is\_constrained) <br>`is_constrained` _&lt;IndexT&gt;[0,1] attribute, indicates if the_**instance** _or_**vertex** _is constrained._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (is\_dynamic) <br>`is_dynamic` _&lt;IndexT&gt;[0,1] attribute, indicates if the_**instance** _or_**vertex** _is is dynamic._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (volume) <br>`volume` _&lt;Float&gt; attribute on_**vertices** _._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (mass\_density) <br>`mass_density` _&lt;Float&gt; attribute on_**vertices** _or_**meta** _._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (gravity) <br>`gravity` _&lt;Vector3&gt; attribute on_**instance** _or_**vertices** _._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (thickness) <br>`thickness` _&lt;Float&gt; attribute on_**vertices** _to indicate the shell thickness (radius) of the vertices which is valid when dealing with codimensional geometries._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (backend\_fem\_vertex\_offset) <br>`backend_fem_vertex_offset` _&lt;IndexT&gt; attribute on_**meta** _to indicate the offset of the vertex in the FEM system._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (backend\_abd\_body\_offset) <br>`backend_abd_body_offset` _&lt;IndexT&gt; attribute on_**meta** _to indicate the offset of the body(instance) in the ABD system._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (dof\_offset) <br>`dof_offset` _&lt;IndexT&gt; attribute on_**meta** _to indicate the degree of freedom offset of this geometry in the whole system._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (dof\_count) <br>`dof_count` _&lt;IndexT&gt; attribute on_**meta** _to indicate the degree of freedom count of this geometry in the whole system._ |
|   | [**UIPC\_BUILTIN\_ATTRIBUTE**](#function-uipc_builtin_attribute) (self\_collision) <br>`self_collision` _&lt;IndexT&gt;[0,1] attribute on_**meta** _to indicate if the geometry needs self-collision detection._ |




























## Public Attributes Documentation




### variable AbstractSimplicialComplex 

```C++
std::string_view uipc::builtin::AbstractSimplicialComplex;
```




<hr>



### variable AffineBody 

```C++
std::string_view uipc::builtin::AffineBody;
```




<hr>



### variable Constraint 

```C++
std::string_view uipc::builtin::Constraint;
```




<hr>



### variable FiniteElement 

```C++
std::string_view uipc::builtin::FiniteElement;
```




<hr>



### variable Geometry 

```C++
std::string_view uipc::builtin::Geometry;
```




<hr>



### variable ImplicitGeometry 

```C++
std::string_view uipc::builtin::ImplicitGeometry;
```




<hr>



### variable InterAffineBody 

```C++
std::string_view uipc::builtin::InterAffineBody;
```




<hr>



### variable SimplicialComplex 

```C++
std::string_view uipc::builtin::SimplicialComplex;
```




<hr>



### variable \_\_data\_\_ 

```C++
std::string_view uipc::builtin::__data__;
```




<hr>



### variable \_\_meta\_\_ 

```C++
std::string_view uipc::builtin::__meta__;
```




<hr>
## Public Functions Documentation




### function UIPC\_BUILTIN\_ATTRIBUTE 

`topo` _attribute on_**vertices** _/_**edges** _/_**triangles** _/_**tetrahedra** _... to indicate the topological type of the element._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    topo
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`position` _&lt;Vector3&gt; attribute on_**vertices** __
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    position
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`velocity` _&lt;Vector3&gt; attribute on_**vertices** _or_`velocity` _&lt;Matrix4x4&gt; attribute on_**instances** _(the derivative of the transform matrix)._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    velocity
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`aim_position` _&lt;Vector3&gt; attribute on_**vertices** _, indicates the aim position of the vertices if the vertices are animated._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    aim_position
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`transform` _&lt;Matrix4x4&gt; attribute on_**instances** __
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    transform
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`aim_transform` _&lt;Matrix4x4&gt; attribute on_**instances** _, indicates the aim transform of the instances if the instances are animated._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    aim_transform
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`contact_element_id` _&lt;IndexT&gt; attribute on_**meta** __
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    contact_element_id
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`constitution_uid` _&lt;U64&gt; attribute on_**meta** _, uid is a unique identifier for a constitution which is defined in the libuipc specification._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    constitution_uid
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`extra_constitution_uids` _&lt;VectorXu64&gt; attribute on_**meta** _, extra constitutions that are applied to the geometry._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    extra_constitution_uids
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`constraint_uid` _&lt;U64&gt; attribute on_**meta** _, uid is a unique identifier for a constraint which is defined in the libuipc specification._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    constraint_uid
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`implicit_geometry_uid` _&lt;U64&gt; attribute on_**meta** _, uid is a unique identifier for an implicit geometry which is defined in the libuipc specification._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    implicit_geometry_uid
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`is_surf` _&lt;IndexT&gt; attribute on_**vertices** _/_**edges** _/_**triangles** _/_**tetrahedra** _... to indicate if the element is a surface element._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    is_surf
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`is_facet` _&lt;IndexT&gt; attribute on_**vertices** _/_**edges** _/_**triangles** _/_**tetrahedra** _to indicate if the element is a facet element._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    is_facet
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`orient` _&lt;IndexT&gt;[-1,0,1] attribute on_**triangles** _to indicate the orientation of the triangle._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    orient
) 
```



1) 0 is the default value, which means the orientation is not determined, or the triangle is not a surface triangle. 2) 1 means outward the tetrahedron 3) -1 means inward the tetrahedron. 


        

<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`parent_id` _&lt;IndexT&gt; attribute on_**edges** _/_**triangles** _, indicates the parent simplex id_
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    parent_id
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`is_fixed` _&lt;IndexT&gt;[0,1] attribute, indicates if the_**instance** _or_**vertex** _is fixed._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    is_fixed
) 
```



'Fixed' means the vertices are not influenced by its constitution and kinetic, keeping the position unchanged. They may be fixed with a certain position, or they are animated with a certain aim position.


1) 0 means the instance or vertex is not fixed. 2) 1 means the instance or vertex is fixed. 


        

<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`is_constrained` _&lt;IndexT&gt;[0,1] attribute, indicates if the_**instance** _or_**vertex** _is constrained._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    is_constrained
) 
```



'Constrained' means the instances or vertices are trying to obey the constraints.


1) 0 means the instance or vertex is not constrained. 2) 1 means the instance or vertex is constrained. 


        

<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`is_dynamic` _&lt;IndexT&gt;[0,1] attribute, indicates if the_**instance** _or_**vertex** _is is dynamic._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    is_dynamic
) 
```



'Dynamic' means the kinetic of instances or vertices is considered.


1) 0 means the the kinetic of the instance or vertex is not considered. 2) 1 means the the kinetic of the instance or vertex is considered. 


        

<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`volume` _&lt;Float&gt; attribute on_**vertices** _._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    volume
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`mass_density` _&lt;Float&gt; attribute on_**vertices** _or_**meta** _._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    mass_density
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`gravity` _&lt;Vector3&gt; attribute on_**instance** _or_**vertices** _._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    gravity
) 
```



If attribute exists, backend will take this value as the gravity of the instance or vertices, instead of the global gravity set in the scene configuration. 


        

<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`thickness` _&lt;Float&gt; attribute on_**vertices** _to indicate the shell thickness (radius) of the vertices which is valid when dealing with codimensional geometries._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    thickness
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`backend_fem_vertex_offset` _&lt;IndexT&gt; attribute on_**meta** _to indicate the offset of the vertex in the FEM system._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    backend_fem_vertex_offset
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`backend_abd_body_offset` _&lt;IndexT&gt; attribute on_**meta** _to indicate the offset of the body(instance) in the ABD system._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    backend_abd_body_offset
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`dof_offset` _&lt;IndexT&gt; attribute on_**meta** _to indicate the degree of freedom offset of this geometry in the whole system._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    dof_offset
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`dof_count` _&lt;IndexT&gt; attribute on_**meta** _to indicate the degree of freedom count of this geometry in the whole system._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    dof_count
) 
```




<hr>



### function UIPC\_BUILTIN\_ATTRIBUTE 

`self_collision` _&lt;IndexT&gt;[0,1] attribute on_**meta** _to indicate if the geometry needs self-collision detection._
```C++
uipc::builtin::UIPC_BUILTIN_ATTRIBUTE (
    self_collision
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/builtin/attribute_name.h`

