

# Namespace uipc::geometry



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**AbstractSimplicialComplex**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md) <br>_Represents an abstract simplicial complex, containing vertices, edges, triangles, and tetrahedra._  |
| class | [**Attribute**](classuipc_1_1geometry_1_1_attribute.md) &lt;typename T&gt;<br>_Template class to represent a geometries attribute of type T._  |
| class | [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) <br>_A collection of geometries attributes._  |
| class | [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md) <br> |
| class | [**AttributeFriend**](classuipc_1_1geometry_1_1_attribute_friend.md) &lt;typename T&gt;<br> |
| class | [**AttributeIO**](classuipc_1_1geometry_1_1_attribute_i_o.md) <br> |
| class | [**AttributeIOError**](classuipc_1_1geometry_1_1_attribute_i_o_error.md) <br> |
| class | [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md) &lt;typename T&gt;<br>_Template class to represent a geometries attribute slot of type T in a geometries attribute collection._  |
| class | [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) <br>_A base geometries class that contains the instance attributes and the meta attributes._  |
| class | [**GeometryAttributeError**](classuipc_1_1geometry_1_1_geometry_attribute_error.md) <br> |
| class | [**GeometryCollection**](classuipc_1_1geometry_1_1_geometry_collection.md) <br> |
| class | [**GeometryFriend**](classuipc_1_1geometry_1_1_geometry_friend.md) &lt;typename T&gt;<br> |
| class | [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) <br> |
| class | [**GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md) &lt;GeometryT&gt;<br> |
| class | [**GeometrySlotT&lt; ImplicitGeometry &gt;**](classuipc_1_1geometry_1_1_geometry_slot_t_3_01_implicit_geometry_01_4.md) &lt;&gt;<br> |
| class | [**GeometrySlotT&lt; SimplicialComplex &gt;**](classuipc_1_1geometry_1_1_geometry_slot_t_3_01_simplicial_complex_01_4.md) &lt;&gt;<br> |
| class | [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) <br>_An abstract class to represent a geometries attribute._  |
| class | [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) <br>_An abstract class to represent a geometries attribute slot in a geometries attribute collection._  |
| class | [**IGeometry**](classuipc_1_1geometry_1_1_i_geometry.md) <br>_An abstract class for geometries._  |
| class | [**IGeometryCollection**](classuipc_1_1geometry_1_1_i_geometry_collection.md) <br> |
| class | [**ImplicitGeometry**](classuipc_1_1geometry_1_1_implicit_geometry.md) <br> |
| class | [**SimplexUtils**](classuipc_1_1geometry_1_1_simplex_utils.md) <br> |
| class | [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) <br>_A simplicial complex is a collection of simplices._  |
| class | [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) &lt;IsConst, N&gt;<br> |
| class | [**SimplicialComplexIO**](classuipc_1_1geometry_1_1_simplicial_complex_i_o.md) <br>_A class for reading and writing simplicial complex._  |
| class | [**SpreadSheetIO**](classuipc_1_1geometry_1_1_spread_sheet_i_o.md) <br>_A class for writing geometry spreadsheet._  |


## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**GeometrySlotState**](#enum-geometryslotstate)  <br> |
| typedef [**GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md)&lt; [**ImplicitGeometry**](classuipc_1_1geometry_1_1_implicit_geometry.md) &gt; | [**ImplicitGeometrySlot**](#typedef-implicitgeometryslot)  <br> |
| typedef [**GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md)&lt; [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) &gt; | [**SimplicialComplexSlot**](#typedef-simplicialcomplexslot)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  UIPC\_GEOMETRY\_API vector&lt; [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) &gt; | [**apply\_region**](#function-apply_region) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & complex) <br>_Take apart the simplicial complex by regions._  |
|  UIPC\_GEOMETRY\_API vector&lt; [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) &gt; | [**apply\_transform**](#function-apply_transform) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & complex) <br>_Apply the instance transform to the simplicial complex._  |
|  UIPC\_GEOMETRY\_API S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; Float &gt; &gt; | [**compute\_vertex\_mass**](#function-compute_vertex_mass) ([**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & R, Float mass\_density) <br> |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**extract\_surface**](#function-extract_surface) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & src) <br>_Extract the surface of a tetrahedral mesh._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**extract\_surface**](#function-extract_surface) (span&lt; const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) \* &gt; complexes) <br>_Extract the surface of a list of tetrahedral meshes and merge them into one._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**facet\_closure**](#function-facet_closure) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & complex) <br>_Generate the closure from a collection of facet simplices, who only have the top dimension simplices._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**flip\_inward\_triangles**](#function-flip_inward_triangles) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc) <br>_Flip the orientation of the triangles in the simplicial complex._  |
|  UIPC\_GEOMETRY\_API [**ImplicitGeometry**](classuipc_1_1geometry_1_1_implicit_geometry.md) | [**ground**](#function-ground) (Float height=0.0, const Vector3 & N=Vector3::UnitY()) <br>_Create a gound plane._  |
|  UIPC\_GEOMETRY\_API [**ImplicitGeometry**](classuipc_1_1geometry_1_1_implicit_geometry.md) | [**halfplane**](#function-halfplane) (const Vector3 & P=Vector3::Zero(), const Vector3 & N=Vector3::UnitY()) <br>_Create a half-plane._  |
|  UIPC\_GEOMETRY\_API S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; IndexT &gt; &gt; | [**label\_connected\_vertices**](#function-label_connected_vertices) ([**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & complex) <br>_Label the connected vertices of a simplicial complex (by edges)._  |
|  UIPC\_GEOMETRY\_API void | [**label\_region**](#function-label_region) ([**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & complex) <br>_Label the regions of a simplicial complex._  |
|  UIPC\_GEOMETRY\_API void | [**label\_surface**](#function-label_surface) ([**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & R) <br>_Label the surface of a simplicial complex._  |
|  UIPC\_GEOMETRY\_API S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; IndexT &gt; &gt; | [**label\_triangle\_orient**](#function-label_triangle_orient) ([**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc) <br>_Label the orientation of the triangles in the simplicial complex._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**linemesh**](#function-linemesh) (span&lt; const Vector3 &gt; Vs, span&lt; const Vector2i &gt; Es) <br>_Create a simplicial complex from a line mesh._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**merge**](#function-merge) (span&lt; const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) \* &gt; complexes) <br>_Merge a list of simplicial complexes into one simplicial complex._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**merge**](#function-merge) (std::initializer\_list&lt; const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) \* &gt; && complexes) <br> |
|  void UIPC\_GEOMETRY\_API | [**mesh\_partition**](#function-mesh_partition) ([**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc, SizeT part\_max\_size) <br>_partition the simplicial complex_  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**pointcloud**](#function-pointcloud) (span&lt; const Vector3 &gt; Vs) <br>_Create a simplicial complex from a point cloud._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**tetmesh**](#function-tetmesh) (span&lt; const Vector3 &gt; Vs, span&lt; const Vector4i &gt; Ts) <br>_Create a simplicial complex from a tetrahedral mesh._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**tetrahedralize**](#function-tetrahedralize) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc, const Json & options=Json::object()) <br>_Tetrahedralize a 2D simplicial complex (trimesh)._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**trimesh**](#function-trimesh) (span&lt; const Vector3 &gt; Vs, span&lt; const Vector3i &gt; Fs) <br>_Create a simplicial complex from a triangle mesh._  |




























## Public Types Documentation




### enum GeometrySlotState 

```C++
enum uipc::geometry::GeometrySlotState {
    Normal,
    PendingCreate,
    PendingDestroy
};
```




<hr>



### typedef ImplicitGeometrySlot 

```C++
using uipc::geometry::ImplicitGeometrySlot = typedef GeometrySlotT<ImplicitGeometry>;
```




<hr>



### typedef SimplicialComplexSlot 

```C++
using uipc::geometry::SimplicialComplexSlot = typedef GeometrySlotT<SimplicialComplex>;
```




<hr>
## Public Functions Documentation




### function apply\_region 

_Take apart the simplicial complex by regions._ 
```C++
UIPC_GEOMETRY_API vector< SimplicialComplex > uipc::geometry::apply_region (
    const SimplicialComplex & complex
) 
```





**Returns:**

vector&lt;SimplicialComplex&gt; The simplicial complexes by regions. 





        

<hr>



### function apply\_transform 

_Apply the instance transform to the simplicial complex._ 
```C++
UIPC_GEOMETRY_API vector< SimplicialComplex > uipc::geometry::apply_transform (
    const SimplicialComplex & complex
) 
```



1) Vertex position of the result simplicial complex will be transformed. 2) The rest meta/instance/vertex/edge/face/tetrahedron attributes will be kept.




**Returns:**

vector&lt;SimplicialComplex&gt; the transformed simplicial complexes. 





        

<hr>



### function compute\_vertex\_mass 

```C++
UIPC_GEOMETRY_API S< AttributeSlot < Float > > uipc::geometry::compute_vertex_mass (
    SimplicialComplex & R,
    Float mass_density
) 
```




<hr>



### function extract\_surface 

_Extract the surface of a tetrahedral mesh._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::extract_surface (
    const SimplicialComplex & src
) 
```





**Parameters:**


* `src` The tetrahedral mesh. 



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) The surface of the tetrahedral mesh. 





        

<hr>



### function extract\_surface 

_Extract the surface of a list of tetrahedral meshes and merge them into one._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::extract_surface (
    span< const SimplicialComplex * > complexes
) 
```



All the instances of the input tetrahedral meshes will be applied to the output surface.




**Parameters:**


* `complexes` The list of tetrahedral meshes. 



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) The surface of the tetrahedral meshes. 





        

<hr>



### function facet\_closure 

_Generate the closure from a collection of facet simplices, who only have the top dimension simplices._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::facet_closure (
    const SimplicialComplex & complex
) 
```



E.g. 1) the input 3D tetmesh can only have tetrahedrons (no triangles, edges). 2) the input 2D trimesh can only have triangles (no edges). 3) the input 1D linemesh can only have edges. 4) the input 0D pointcloud can only have vertices. 


        

<hr>



### function flip\_inward\_triangles 

_Flip the orientation of the triangles in the simplicial complex._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::flip_inward_triangles (
    const SimplicialComplex & sc
) 
```



The input simplicial complex should have the attribute slot 'orient':&lt;Index&gt; for each triangle. After the operation, the orientation of the triangles will be flipped, and the `orient` attribute will be updated.




**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) the simplicial complex with the orientation of the triangles flipped. 





        

<hr>



### function ground 

_Create a gound plane._ 
```C++
UIPC_GEOMETRY_API ImplicitGeometry uipc::geometry::ground (
    Float height=0.0,
    const Vector3 & N=Vector3::UnitY()
) 
```





**Parameters:**


* `height` The height of the ground plane 




        

<hr>



### function halfplane 

_Create a half-plane._ 
```C++
UIPC_GEOMETRY_API ImplicitGeometry uipc::geometry::halfplane (
    const Vector3 & P=Vector3::Zero(),
    const Vector3 & N=Vector3::UnitY()
) 
```





**Parameters:**


* `height` The height of the ground plane 




        

<hr>



### function label\_connected\_vertices 

_Label the connected vertices of a simplicial complex (by edges)._ 
```C++
UIPC_GEOMETRY_API S< AttributeSlot < IndexT > > uipc::geometry::label_connected_vertices (
    SimplicialComplex & complex
) 
```




* Create a `region` &lt;IndexT&gt; attribute on `vertices` to tell which region a vertex is belong to.
* Create a `region_count` &lt;IndexT&gt; attribute on `meta` to tell how many regions are there.






**Returns:**

S&lt;AttributeSlot&lt;IndexT&gt;&gt; The `region` attribute slot. 





        

<hr>



### function label\_region 

_Label the regions of a simplicial complex._ 
```C++
UIPC_GEOMETRY_API void uipc::geometry::label_region (
    SimplicialComplex & complex
) 
```




* Create a `region` &lt;IndexT&gt; attribute on `edges` to tell which region an edge is belong to.
* Create a `region` &lt;IndexT&gt; attribute on `triangles` to tell which region a triangle is belong to. (if exists)
* Create a `region` &lt;IndexT&gt; attribute on `tetrahedra` to tell which region a tetrahedron is belong to. (if exists)
* Create a `region_count` &lt;IndexT&gt; attribute on `meta` to tell how many regions are there.






**Returns:**

S&lt;AttributeSlot&lt;IndexT&gt;&gt; The `region` attribute slot. 





        

<hr>



### function label\_surface 

_Label the surface of a simplicial complex._ 
```C++
UIPC_GEOMETRY_API void uipc::geometry::label_surface (
    SimplicialComplex & R
) 
```



1) label 'is\_surf':&lt;IndexT&gt; on vertices/edges/triangles/tetrahedra 2) set 'parent\_id':&lt;IndexT&gt; on triangles, indicating the parent tetrahedron




**Parameters:**


* `R` the simplicial complex to be labeled. 




        

<hr>



### function label\_triangle\_orient 

_Label the orientation of the triangles in the simplicial complex._ 
```C++
UIPC_GEOMETRY_API S< AttributeSlot < IndexT > > uipc::geometry::label_triangle_orient (
    SimplicialComplex & sc
) 
```



Set 'orient':&lt;Index&gt; for each triangle in the simplicial complex. 1) orient=1 means the triangle is oriented outward the tetrahedron. 2) orient=0 means the orientation is undetermined. 3) orient=-1 means the triangle is oriented inward the tetrahedron.




**Returns:**

P&lt;AttributeSlot&lt;IndexT&gt;&gt; the attribute slot of the triangle orientation. 





        

<hr>



### function linemesh 

_Create a simplicial complex from a line mesh._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::linemesh (
    span< const Vector3 > Vs,
    span< const Vector2i > Es
) 
```





**Parameters:**


* `Vs` The vertex positions of the line mesh 
* `Es` The edges of the line mesh 



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) 





        

<hr>



### function merge 

_Merge a list of simplicial complexes into one simplicial complex._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::merge (
    span< const SimplicialComplex * > complexes
) 
```



All input simplicial complexes must have only one instance.




**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) the merged simplicial complex. 





        

<hr>



### function merge 

```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::merge (
    std::initializer_list< const SimplicialComplex * > && complexes
) 
```




<hr>



### function mesh\_partition 

_partition the simplicial complex_ 
```C++
void UIPC_GEOMETRY_API uipc::geometry::mesh_partition (
    SimplicialComplex & sc,
    SizeT part_max_size
) 
```



create a `mesh_part` &lt;IndexT&gt; attribute on the simplicial complex' vertices




**Parameters:**


* `sc` simplicial complex 
* `part_max_size` the vertex number in each partition &lt;= part\_max\_size 




        

<hr>



### function pointcloud 

_Create a simplicial complex from a point cloud._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::pointcloud (
    span< const Vector3 > Vs
) 
```





**Parameters:**


* `Vs` The vertex positions of the point cloud 



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) 





        

<hr>



### function tetmesh 

_Create a simplicial complex from a tetrahedral mesh._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::tetmesh (
    span< const Vector3 > Vs,
    span< const Vector4i > Ts
) 
```





**Parameters:**


* `Vs` The vertex positions of the tetrahedral mesh 
* `Ts` The tetrahedra of the tetrahedral mesh 




        

<hr>



### function tetrahedralize 

_Tetrahedralize a 2D simplicial complex (trimesh)._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::tetrahedralize (
    const SimplicialComplex & sc,
    const Json & options=Json::object()
) 
```





**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) The simplicial complexes by regions. 





        

<hr>



### function trimesh 

_Create a simplicial complex from a triangle mesh._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::trimesh (
    span< const Vector3 > Vs,
    span< const Vector3i > Fs
) 
```





**Parameters:**


* `Vs` The vertex positions of the triangle mesh 
* `Fs` The triangles of the triangle mesh 



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/backend/visitors/geometry_visitor.h`

