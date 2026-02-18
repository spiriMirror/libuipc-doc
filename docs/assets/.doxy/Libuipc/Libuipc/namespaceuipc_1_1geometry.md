

# Namespace uipc::geometry



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**affine\_body**](namespaceuipc_1_1geometry_1_1affine__body.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**AbstractSimplicialComplex**](classuipc_1_1geometry_1_1AbstractSimplicialComplex.md) <br>_Represents an abstract simplicial complex, containing vertices, edges, triangles, and tetrahedra._  |
| class | [**Attribute**](classuipc_1_1geometry_1_1Attribute.md) &lt;typename T&gt;<br>_Template class to represent a geometries attribute of type T._  |
| class | [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) <br>_A collection of geometries attributes._  |
| class | [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) <br> |
| class | [**AttributeCollectionError**](classuipc_1_1geometry_1_1AttributeCollectionError.md) <br> |
| class | [**AttributeCollectionFactory**](classuipc_1_1geometry_1_1AttributeCollectionFactory.md) <br> |
| class | [**AttributeCopy**](classuipc_1_1geometry_1_1AttributeCopy.md) <br> |
| class | [**AttributeDebugInfo**](classuipc_1_1geometry_1_1AttributeDebugInfo.md) <br> |
| class | [**AttributeFactory**](classuipc_1_1geometry_1_1AttributeFactory.md) <br> |
| class | [**AttributeFriend**](classuipc_1_1geometry_1_1AttributeFriend.md) &lt;typename T&gt;<br> |
| class | [**AttributeIO**](classuipc_1_1geometry_1_1AttributeIO.md) <br> |
| class | [**AttributeIOError**](classuipc_1_1geometry_1_1AttributeIOError.md) <br> |
| class | [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md) &lt;typename T&gt;<br>_Template class to represent a geometries attribute slot of type T in a geometries attribute collection._  |
| class | [**BVH**](classuipc_1_1geometry_1_1BVH.md) <br> |
| class | [**DeserialSharedAttributeContext**](classuipc_1_1geometry_1_1DeserialSharedAttributeContext.md) <br> |
| class | [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) <br>_A base geometries class that contains the instance attributes and the meta attributes._  |
| class | [**GeometryAtlas**](classuipc_1_1geometry_1_1GeometryAtlas.md) <br> |
| class | [**GeometryAtlasCommit**](classuipc_1_1geometry_1_1GeometryAtlasCommit.md) <br> |
| class | [**GeometryCollection**](classuipc_1_1geometry_1_1GeometryCollection.md) <br> |
| class | [**GeometryCollectionCommit**](classuipc_1_1geometry_1_1GeometryCollectionCommit.md) <br> |
| class | [**GeometryCommit**](classuipc_1_1geometry_1_1GeometryCommit.md) <br> |
| class | [**GeometryFactory**](classuipc_1_1geometry_1_1GeometryFactory.md) <br> |
| class | [**GeometryFriend**](classuipc_1_1geometry_1_1GeometryFriend.md) &lt;typename T&gt;<br> |
| class | [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) <br> |
| class | [**GeometrySlotT**](classuipc_1_1geometry_1_1GeometrySlotT.md) &lt;GeometryT&gt;<br> |
| class | [**GeometrySlotT&lt; Geometry &gt;**](classuipc_1_1geometry_1_1GeometrySlotT_3_01Geometry_01_4.md) &lt;&gt;<br> |
| class | [**GeometrySlotT&lt; ImplicitGeometry &gt;**](classuipc_1_1geometry_1_1GeometrySlotT_3_01ImplicitGeometry_01_4.md) &lt;&gt;<br> |
| class | [**GeometrySlotT&lt; SimplicialComplex &gt;**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &lt;&gt;<br> |
| class | [**IAttribute**](classuipc_1_1geometry_1_1IAttribute.md) <br>_An abstract class to represent a geometries attribute._  |
| class | [**IAttributeSlot**](classuipc_1_1geometry_1_1IAttributeSlot.md) <br>_An abstract class to represent a geometries attribute slot in a geometries attribute collection._  |
| class | [**IGeometry**](classuipc_1_1geometry_1_1IGeometry.md) <br>_An abstract class for geometries._  |
| class | [**IGeometryCollection**](classuipc_1_1geometry_1_1IGeometryCollection.md) <br> |
| class | [**ImplicitGeometry**](classuipc_1_1geometry_1_1ImplicitGeometry.md) <br> |
| class | [**Octree**](classuipc_1_1geometry_1_1Octree.md) <br> |
| class | [**SerialSharedAttributeContext**](classuipc_1_1geometry_1_1SerialSharedAttributeContext.md) <br> |
| class | [**SimplexUtils**](classuipc_1_1geometry_1_1SimplexUtils.md) <br> |
| class | [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) <br>_A simplicial complex is a collection of simplices._  |
| class | [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1SimplicialComplexAttributes.md) &lt;IsConst, N&gt;<br> |
| class | [**SimplicialComplexIO**](classuipc_1_1geometry_1_1SimplicialComplexIO.md) <br>_A class for reading and writing simplicial complex._  |
| class | [**SpreadSheetIO**](classuipc_1_1geometry_1_1SpreadSheetIO.md) <br>_A class for writing geometry spreadsheet._  |


## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**GeometrySlotState**](#enum-geometryslotstate)  <br> |
| typedef [**GeometrySlotT**](classuipc_1_1geometry_1_1GeometrySlotT.md)&lt; [**ImplicitGeometry**](classuipc_1_1geometry_1_1ImplicitGeometry.md) &gt; | [**ImplicitGeometrySlot**](#typedef-implicitgeometryslot)  <br> |
| typedef [**GeometrySlotT**](classuipc_1_1geometry_1_1GeometrySlotT.md)&lt; [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) &gt; | [**SimplicialComplexSlot**](#typedef-simplicialcomplexslot)  <br> |
| typedef std::chrono::time\_point&lt; std::chrono::high\_resolution\_clock &gt; | [**TimePoint**](#typedef-timepoint)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  UIPC\_GEOMETRY\_API vector&lt; [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) &gt; | [**apply\_region**](#function-apply_region) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & complex) <br>_Take apart the simplicial complex by regions._  |
|  UIPC\_GEOMETRY\_API vector&lt; [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) &gt; | [**apply\_transform**](#function-apply_transform) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & complex) <br>_Apply the instance transform to the simplicial complex._  |
|  UIPC\_CORE\_API void | [**check\_view**](#function-check_view) (const [**IAttributeSlot**](classuipc_1_1geometry_1_1IAttributeSlot.md) \* slot) <br> |
|  UIPC\_GEOMETRY\_API S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; Float &gt; &gt; | [**compute\_mesh\_d\_hat**](#function-compute_mesh_d_hat) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & R, Float max\_d\_hat=std::numeric\_limits&lt; Float &gt;::max()) <br>_Suggest a proper d\_hat for a mesh, create an attribute_ `d_hat` _on meta._ |
|  UIPC\_GEOMETRY\_API Float | [**compute\_mesh\_volume**](#function-compute_mesh_volume) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & R) <br>_Compute the volume of the simplicial complex._  |
|  UIPC\_GEOMETRY\_API S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; Float &gt; &gt; | [**compute\_vertex\_volume**](#function-compute_vertex_volume) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & R) <br> |
|  UIPC\_GEOMETRY\_API std::string | [**constitution\_type**](#function-constitution_type) (const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & geo) <br> |
|  Float UIPC\_GEOMETRY\_API | [**edge\_edge\_squared\_distance**](#function-edge_edge_squared_distance) (const Vector3 & Ea0, const Vector3 & Ea1, const Vector3 & Eb0, const Vector3 & Eb1) <br> |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**extract\_surface**](#function-extract_surface) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & src) <br>_Extract the surface of a tetrahedral mesh._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**extract\_surface**](#function-extract_surface) (span&lt; const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) \* &gt; complexes) <br>_Extract the surface of a list of tetrahedral meshes and merge them into one._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**facet\_closure**](#function-facet_closure) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & complex) <br>_Generate the closure from a collection of facet simplices, who only have the top dimension simplices._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**flip\_inward\_triangles**](#function-flip_inward_triangles) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc) <br>_Flip the orientation of the triangles in the simplicial complex._  |
|  UIPC\_GEOMETRY\_API [**ImplicitGeometry**](classuipc_1_1geometry_1_1ImplicitGeometry.md) | [**ground**](#function-ground) (Float height=0.0, const Vector3 & N=Vector3::UnitY()) <br>_Create a gound plane._  |
|  UIPC\_GEOMETRY\_API [**ImplicitGeometry**](classuipc_1_1geometry_1_1ImplicitGeometry.md) | [**halfplane**](#function-halfplane) (const Vector3 & P=Vector3::Zero(), const Vector3 & N=Vector3::UnitY()) <br>_Create a half-plane._  |
|  Float UIPC\_GEOMETRY\_API | [**halfplane\_vertex\_signed\_distance**](#function-halfplane_vertex_signed_distance) (const Vector3 & P, const Vector3 & N, const Vector3 & V, Float V\_thickness=0.0) <br>_Compute the distance between a half-plane (P, N) and a vertex V (with thickness V\_thickness)._  |
|  UIPC\_GEOMETRY\_API bool | [**is\_point\_in\_tet**](#function-is_point_in_tet) (const Vector3 & T0, const Vector3 & T1, const Vector3 & T2, const Vector3 & T3, const Vector3 & P) <br>_Check if a point is in a tetrahedron._  |
|  UIPC\_GEOMETRY\_API bool | [**is\_trimesh\_closed**](#function-is_trimesh_closed) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & R) <br>_Check if a trimesh is closed._  |
|  UIPC\_GEOMETRY\_API S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; IndexT &gt; &gt; | [**label\_connected\_vertices**](#function-label_connected_vertices) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & complex) <br>_Label the connected vertices of a simplicial complex (by edges)._  |
|  UIPC\_GEOMETRY\_API S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; IndexT &gt; &gt; | [**label\_graph\_color**](#function-label_graph_color) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc) <br>_Label the vertex color of a simplicial complex by graph coloring algorithm._  |
|  UIPC\_GEOMETRY\_API S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; IndexT &gt; &gt; | [**label\_open\_edge**](#function-label_open_edge) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & R) <br>_Label open edges in a trimesh._  |
|  UIPC\_GEOMETRY\_API void | [**label\_region**](#function-label_region) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & complex) <br>_Label the regions of a simplicial complex._  |
|  UIPC\_GEOMETRY\_API void | [**label\_surface**](#function-label_surface) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & R) <br>_Label the surface of a simplicial complex._  |
|  UIPC\_GEOMETRY\_API S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; IndexT &gt; &gt; | [**label\_triangle\_orient**](#function-label_triangle_orient) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc) <br>_Label the orientation of the triangles in the simplicial complex._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**linemesh**](#function-linemesh) (span&lt; const Vector3 &gt; Vs, span&lt; const Vector2i &gt; Es) <br>_Create a simplicial complex from a line mesh._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**merge**](#function-merge) (span&lt; const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) \* &gt; complexes) <br>_Merge a list of simplicial complexes into one simplicial complex._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**merge**](#function-merge) (span&lt; const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) &gt; complexes) <br> |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**merge**](#function-merge) (std::initializer\_list&lt; const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) \* &gt; && complexes) <br> |
|  void UIPC\_GEOMETRY\_API | [**mesh\_partition**](#function-mesh_partition) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, SizeT part\_max\_size) <br>_partition the simplicial complex_  |
|  UIPC\_CORE\_API [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) & | [**operator+=**](#function-operator) ([**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) & dst, const [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) & inc) <br> |
|  UIPC\_CORE\_API [**GeometryCollection**](classuipc_1_1geometry_1_1GeometryCollection.md) & | [**operator+=**](#function-operator_1) ([**GeometryCollection**](classuipc_1_1geometry_1_1GeometryCollection.md) & dst, const [**GeometryCollectionCommit**](classuipc_1_1geometry_1_1GeometryCollectionCommit.md) & inc) <br> |
|  UIPC\_CORE\_API [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & | [**operator+=**](#function-operator_2) ([**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & base, const [**GeometryCommit**](classuipc_1_1geometry_1_1GeometryCommit.md) & inc) <br> |
|  UIPC\_CORE\_API [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) | [**operator-**](#function-operator-) (const [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) & dst, const [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) & src) <br> |
|  UIPC\_CORE\_API [**GeometryCollectionCommit**](classuipc_1_1geometry_1_1GeometryCollectionCommit.md) | [**operator-**](#function-operator-_1) (const [**GeometryCollection**](classuipc_1_1geometry_1_1GeometryCollection.md) & dst, const [**GeometryCollection**](classuipc_1_1geometry_1_1GeometryCollection.md) & src) <br> |
|  UIPC\_CORE\_API [**GeometryCommit**](classuipc_1_1geometry_1_1GeometryCommit.md) | [**operator-**](#function-operator-_2) (const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & dst, const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & src) <br> |
|  UIPC\_GEOMETRY\_API Matrix4x4 | [**optimal\_transform**](#function-optimal_transform) (span&lt; const Vector3 &gt; S, span&lt; const Vector3 &gt; D) <br>_Find out the optimal transformation matrix that maps the source points to the destination points._  |
|  UIPC\_GEOMETRY\_API Matrix4x4 | [**optimal\_transform**](#function-optimal_transform) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & S, const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & D) <br>_Find out the optimal transformation matrix that maps the source simplicial complex to the destination simplicial complex._  |
|  Float UIPC\_GEOMETRY\_API | [**point\_edge\_squared\_distance**](#function-point_edge_squared_distance) (const Vector3 & P, const Vector3 & E0, const Vector3 & E1) <br> |
|  Float UIPC\_GEOMETRY\_API | [**point\_point\_squared\_distance**](#function-point_point_squared_distance) (const Vector3 & P0, const Vector3 & P1) <br> |
|  Float UIPC\_GEOMETRY\_API | [**point\_triangle\_squared\_distance**](#function-point_triangle_squared_distance) (const Vector3 & P, const Vector3 & T0, const Vector3 & T1, const Vector3 & T2) <br> |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**pointcloud**](#function-pointcloud) (span&lt; const Vector3 &gt; Vs) <br>_Create a simplicial complex from a point cloud._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**points\_from\_volume**](#function-points_from_volume) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float resolution=0.01) <br>_Construct a point cloud inside a volume represented by a simplicial complex._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**tetmesh**](#function-tetmesh) (span&lt; const Vector3 &gt; Vs, span&lt; const Vector4i &gt; Ts) <br>_Create a simplicial complex from a tetrahedral mesh._  |
|  UIPC\_GEOMETRY\_API bool | [**tri\_edge\_intersect**](#function-tri_edge_intersect) (const Vector3 & T0, const Vector3 & T1, const Vector3 & T2, const Vector3 & E0, const Vector3 & E1) <br>_Check if a triangle and an edge intersect._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**trimesh**](#function-trimesh) (span&lt; const Vector3 &gt; Vs, span&lt; const Vector3i &gt; Fs) <br>_Create a simplicial complex from a triangle mesh._  |
|  UIPC\_GEOMETRY\_API [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) | [**trimesh**](#function-trimesh) (span&lt; const Vector3 &gt; Vs, span&lt; const Vector4i &gt; Fs) <br>_Create a 2D simplicial complex from a quad mesh (4-sided polygons)._  |




























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



### typedef TimePoint 

```C++
using uipc::geometry::TimePoint = typedef std::chrono::time_point<std::chrono::high_resolution_clock>;
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



### function check\_view 

```C++
UIPC_CORE_API void uipc::geometry::check_view (
    const IAttributeSlot * slot
) 
```




<hr>



### function compute\_mesh\_d\_hat 

_Suggest a proper d\_hat for a mesh, create an attribute_ `d_hat` _on meta._
```C++
UIPC_GEOMETRY_API S< AttributeSlot < Float > > uipc::geometry::compute_mesh_d_hat (
    SimplicialComplex & R,
    Float max_d_hat=std::numeric_limits< Float >::max()
) 
```





**Parameters:**


* `R` The simplicial complex to compute d\_hat for. 
* `max_d_hat` The maximum allowed d\_hat, default to infinity. 




        

<hr>



### function compute\_mesh\_volume 

_Compute the volume of the simplicial complex._ 
```C++
UIPC_GEOMETRY_API Float uipc::geometry::compute_mesh_volume (
    SimplicialComplex & R
) 
```



Only tetmesh and closed trimesh are supported.




**Parameters:**


* `R` The simplicial complex. 



**Returns:**

The volume of the simplicial complex. 





        

<hr>



### function compute\_vertex\_volume 

```C++
UIPC_GEOMETRY_API S< AttributeSlot < Float > > uipc::geometry::compute_vertex_volume (
    SimplicialComplex & R
) 
```




<hr>



### function constitution\_type 

```C++
UIPC_GEOMETRY_API std::string uipc::geometry::constitution_type (
    const Geometry & geo
) 
```




<hr>



### function edge\_edge\_squared\_distance 

```C++
Float UIPC_GEOMETRY_API uipc::geometry::edge_edge_squared_distance (
    const Vector3 & Ea0,
    const Vector3 & Ea1,
    const Vector3 & Eb0,
    const Vector3 & Eb1
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

[**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) The surface of the tetrahedral mesh. 





        

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

[**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) The surface of the tetrahedral meshes. 





        

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

[**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) the simplicial complex with the orientation of the triangles flipped. 





        

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



### function halfplane\_vertex\_signed\_distance 

_Compute the distance between a half-plane (P, N) and a vertex V (with thickness V\_thickness)._ 
```C++
Float UIPC_GEOMETRY_API uipc::geometry::halfplane_vertex_signed_distance (
    const Vector3 & P,
    const Vector3 & N,
    const Vector3 & V,
    Float V_thickness=0.0
) 
```





**Parameters:**


* `P` The Origin point of the half-plane. 
* `N` The Normal vector of the half-plane. 
* `V` The Vertex point. 
* `V_thickness` The thickness of the vertex. 




        

<hr>



### function is\_point\_in\_tet 

_Check if a point is in a tetrahedron._ 
```C++
UIPC_GEOMETRY_API bool uipc::geometry::is_point_in_tet (
    const Vector3 & T0,
    const Vector3 & T1,
    const Vector3 & T2,
    const Vector3 & T3,
    const Vector3 & P
) 
```



T0, T1, T2, T3 the vertices of the tetrahedron P is the point




**Returns:**

true if the point is in the tetrahedron 





        

<hr>



### function is\_trimesh\_closed 

_Check if a trimesh is closed._ 
```C++
UIPC_GEOMETRY_API bool uipc::geometry::is_trimesh_closed (
    const SimplicialComplex & R
) 
```



Only 2D [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) is supported.




**Parameters:**


* `R` the simplicial complex to be checked. 



**Returns:**

true if the trimesh is closed, false otherwise. 





        

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



### function label\_graph\_color 

_Label the vertex color of a simplicial complex by graph coloring algorithm._ 
```C++
UIPC_GEOMETRY_API S< AttributeSlot < IndexT > > uipc::geometry::label_graph_color (
    SimplicialComplex & sc
) 
```



The edges of the graph is from the edges of the simplicial complex.
* Create a `graph/color` &lt;IndexT&gt; attribute on `vertices` to tell the color of each vertex.
* Create a `graph/color_count` &lt;IndexT&gt; attribute on `meta` to tell how many colors are used.






**Returns:**

S&lt;AttributeSlot&lt;IndexT&gt;&gt; The `graph/color` attribute slot. 





        

<hr>



### function label\_open\_edge 

_Label open edges in a trimesh._ 
```C++
UIPC_GEOMETRY_API S< AttributeSlot < IndexT > > uipc::geometry::label_open_edge (
    SimplicialComplex & R
) 
```



An edge is considered open if it is shared by exactly 1 triangle. An edge shared by 2 triangles is a normal closed edge. An edge shared by &gt;=3 triangles is invalid and will throw an exception.



* Create an `is_open` &lt;IndexT&gt; attribute on `edges` to mark which edges are open (1 = open, 0 = closed).




Only 2D [**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) is supported.




**Parameters:**


* `R` the simplicial complex to be checked. 



**Returns:**

S&lt;AttributeSlot&lt;IndexT&gt;&gt; The `is_open` attribute slot. 





        

<hr>



### function label\_region 

_Label the regions of a simplicial complex._ 
```C++
UIPC_GEOMETRY_API void uipc::geometry::label_region (
    SimplicialComplex & complex
) 
```




* Create a `region` &lt;IndexT&gt; attribute on `vertices` to tell which region a vertex belongs to.
* Create a `region` &lt;IndexT&gt; attribute on `edges` to tell which region an edge belongs to.
* Create a `region` &lt;IndexT&gt; attribute on `triangles` (if exists) to tell which region a triangle belongs to.
* Create a `region` &lt;IndexT&gt; attribute on `tetrahedra` (if exists) to tell which region a tetrahedron belongs to.
* Create a `region_count` &lt;IndexT&gt; attribute on `meta` to tell how many regions are there. 




        

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

[**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) 





        

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

[**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) the merged simplicial complex. 





        

<hr>



### function merge 

```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::merge (
    span< const SimplicialComplex > complexes
) 
```




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



### function operator+= 

```C++
UIPC_CORE_API AttributeCollection & uipc::geometry::operator+= (
    AttributeCollection & dst,
    const AttributeCollectionCommit & inc
) 
```




<hr>



### function operator+= 

```C++
UIPC_CORE_API GeometryCollection & uipc::geometry::operator+= (
    GeometryCollection & dst,
    const GeometryCollectionCommit & inc
) 
```




<hr>



### function operator+= 

```C++
UIPC_CORE_API Geometry & uipc::geometry::operator+= (
    Geometry & base,
    const GeometryCommit & inc
) 
```




<hr>



### function operator- 

```C++
UIPC_CORE_API AttributeCollectionCommit uipc::geometry::operator- (
    const AttributeCollection & dst,
    const AttributeCollection & src
) 
```




<hr>



### function operator- 

```C++
UIPC_CORE_API GeometryCollectionCommit uipc::geometry::operator- (
    const GeometryCollection & dst,
    const GeometryCollection & src
) 
```




<hr>



### function operator- 

```C++
UIPC_CORE_API GeometryCommit uipc::geometry::operator- (
    const Geometry & dst,
    const Geometry & src
) 
```




<hr>



### function optimal\_transform 

_Find out the optimal transformation matrix that maps the source points to the destination points._ 
```C++
UIPC_GEOMETRY_API Matrix4x4 uipc::geometry::optimal_transform (
    span< const Vector3 > S,
    span< const Vector3 > D
) 
```





**Parameters:**


* `S` The source points. 
* `D` The destination points. 



**Returns:**







        

<hr>



### function optimal\_transform 

_Find out the optimal transformation matrix that maps the source simplicial complex to the destination simplicial complex._ 
```C++
UIPC_GEOMETRY_API Matrix4x4 uipc::geometry::optimal_transform (
    const SimplicialComplex & S,
    const SimplicialComplex & D
) 
```





**Parameters:**


* `S` The source simplicial complex. 
* `D` The destination simplicial complex. 



**Returns:**







        

<hr>



### function point\_edge\_squared\_distance 

```C++
Float UIPC_GEOMETRY_API uipc::geometry::point_edge_squared_distance (
    const Vector3 & P,
    const Vector3 & E0,
    const Vector3 & E1
) 
```




<hr>



### function point\_point\_squared\_distance 

```C++
Float UIPC_GEOMETRY_API uipc::geometry::point_point_squared_distance (
    const Vector3 & P0,
    const Vector3 & P1
) 
```




<hr>



### function point\_triangle\_squared\_distance 

```C++
Float UIPC_GEOMETRY_API uipc::geometry::point_triangle_squared_distance (
    const Vector3 & P,
    const Vector3 & T0,
    const Vector3 & T1,
    const Vector3 & T2
) 
```




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

[**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) 





        

<hr>



### function points\_from\_volume 

_Construct a point cloud inside a volume represented by a simplicial complex._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::points_from_volume (
    const SimplicialComplex & sc,
    Float resolution=0.01
) 
```





**Parameters:**


* `sc` The input simplicial complex representing a volume (closed manifold). 
* `resolution` The resolution of the point cloud.



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) A point cloud represented as a simplicial complex with only vertices. 





        

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



### function tri\_edge\_intersect 

_Check if a triangle and an edge intersect._ 
```C++
UIPC_GEOMETRY_API bool uipc::geometry::tri_edge_intersect (
    const Vector3 & T0,
    const Vector3 & T1,
    const Vector3 & T2,
    const Vector3 & E0,
    const Vector3 & E1
) 
```



T0, T1, T2 the vertices of the triangle E0, E1 the vertices of the edge




**Returns:**

true if the triangle and the edge intersect 





        

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

[**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) 





        

<hr>



### function trimesh 

_Create a 2D simplicial complex from a quad mesh (4-sided polygons)._ 
```C++
UIPC_GEOMETRY_API SimplicialComplex uipc::geometry::trimesh (
    span< const Vector3 > Vs,
    span< const Vector4i > Fs
) 
```





**Parameters:**


* `Vs` The vertex positions of the quad mesh 
* `Fs` The quads of the quad mesh 



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/backend/visitors/geometry_visitor.h`

