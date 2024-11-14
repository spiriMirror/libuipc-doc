

# Class uipc::geometry::SimplicialComplex



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md)



_A simplicial complex is a collection of simplices._ [More...](#detailed-description)

* `#include <simplicial_complex.h>`



Inherits the following classes: [uipc::geometry::Geometry](classuipc_1_1geometry_1_1_geometry.md)














## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md)&lt; true, 1 &gt; | [**CEdgeAttributes**](#typedef-cedgeattributes)  <br> |
| typedef [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md)&lt; true, 3 &gt; | [**CTetrahedronAttributes**](#typedef-ctetrahedronattributes)  <br> |
| typedef [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md)&lt; true, 2 &gt; | [**CTriangleAttributes**](#typedef-ctriangleattributes)  <br> |
| typedef [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md)&lt; true, 0 &gt; | [**CVertexAttributes**](#typedef-cvertexattributes)  <br> |
| typedef [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md)&lt; false, 1 &gt; | [**EdgeAttributes**](#typedef-edgeattributes)  <br>_Alias for the edge attributes._  |
| typedef [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md)&lt; false, 3 &gt; | [**TetrahedronAttributes**](#typedef-tetrahedronattributes)  <br>_Alias for the tetrahedron attributes._  |
| typedef [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md)&lt; false, 2 &gt; | [**TriangleAttributes**](#typedef-triangleattributes)  <br>_Alias for the triangle attributes._  |
| typedef [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md)&lt; false, 0 &gt; | [**VertexAttributes**](#typedef-vertexattributes)  <br>_Alias for the vertex attributes._  |


## Public Types inherited from uipc::geometry::Geometry

See [uipc::geometry::Geometry](classuipc_1_1geometry_1_1_geometry.md)

| Type | Name |
| ---: | :--- |
| typedef [**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md)&lt; true &gt; | [**CInstanceAttributes**](classuipc_1_1geometry_1_1_geometry.md#typedef-cinstanceattributes)  <br> |
| typedef [**MetaAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_meta_attributes_t.md)&lt; true &gt; | [**CMetaAttributes**](classuipc_1_1geometry_1_1_geometry.md#typedef-cmetaattributes)  <br> |
| typedef [**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md)&lt; false &gt; | [**InstanceAttributes**](classuipc_1_1geometry_1_1_geometry.md#typedef-instanceattributes)  <br> |
| typedef [**MetaAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_meta_attributes_t.md)&lt; false &gt; | [**MetaAttributes**](classuipc_1_1geometry_1_1_geometry.md#typedef-metaattributes)  <br> |


























































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SimplicialComplex**](#function-simplicialcomplex-13) () <br> |
|   | [**SimplicialComplex**](#function-simplicialcomplex-23) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & o) = default<br> |
|   | [**SimplicialComplex**](#function-simplicialcomplex-33) ([**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) && o) = default<br> |
|  IndexT | [**dim**](#function-dim) () noexcept const<br>_Get the dimension of the simplicial complex._  |
|  [**EdgeAttributes**](classuipc_1_1geometry_1_1_simplicial_complex.md#typedef-edgeattributes) | [**edges**](#function-edges-12) () noexcept<br>_A wrapper of the edges and its attributes of the simplicial complex._  |
|  CEdgeAttributes | [**edges**](#function-edges-22) () noexcept const<br> |
|  [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & | [**operator=**](#function-operator) (const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & o) = delete<br> |
|  [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & | [**operator=**](#function-operator_1) ([**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) && o) = delete<br> |
|  [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; Vector3 &gt; & | [**positions**](#function-positions-12) () noexcept<br>_Get the positions of the vertices._  |
|  const [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; Vector3 &gt; & | [**positions**](#function-positions-22) () noexcept const<br>_A short cut to get the positions of the vertices._  |
|  [**TetrahedronAttributes**](classuipc_1_1geometry_1_1_simplicial_complex.md#typedef-tetrahedronattributes) | [**tetrahedra**](#function-tetrahedra-12) () noexcept<br>_A wrapper of the tetrahedra and its attributes of the simplicial complex._  |
|  CTetrahedronAttributes | [**tetrahedra**](#function-tetrahedra-22) () noexcept const<br> |
|  [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; Matrix4x4 &gt; & | [**transforms**](#function-transforms-12) () <br>_A short-cut to get the non-const transforms attribute slot._  |
|  const [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; Matrix4x4 &gt; & | [**transforms**](#function-transforms-22) () const<br>_A short-cut to get the const transforms attribute slot._  |
|  [**TriangleAttributes**](classuipc_1_1geometry_1_1_simplicial_complex.md#typedef-triangleattributes) | [**triangles**](#function-triangles-12) () noexcept<br>_A wrapper of the triangles and its attributes of the simplicial complex._  |
|  CTriangleAttributes | [**triangles**](#function-triangles-22) () noexcept const<br> |
|  [**VertexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex.md#typedef-vertexattributes) | [**vertices**](#function-vertices-12) () noexcept<br>_A wrapper of the vertices and its attributes of the simplicial complex._  |
|  CVertexAttributes | [**vertices**](#function-vertices-22) () noexcept const<br> |


## Public Functions inherited from uipc::geometry::Geometry

See [uipc::geometry::Geometry](classuipc_1_1geometry_1_1_geometry.md)

| Type | Name |
| ---: | :--- |
|   | [**Geometry**](classuipc_1_1geometry_1_1_geometry.md#function-geometry-13) () <br> |
|   | [**Geometry**](classuipc_1_1geometry_1_1_geometry.md#function-geometry-23) (const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & o) = default<br> |
|   | [**Geometry**](classuipc_1_1geometry_1_1_geometry.md#function-geometry-33) ([**Geometry**](classuipc_1_1geometry_1_1_geometry.md) && o) = default<br> |
|  T \* | [**as**](classuipc_1_1geometry_1_1_geometry.md#function-as) () <br> |
|  InstanceAttributes | [**instances**](classuipc_1_1geometry_1_1_geometry.md#function-instances-12) () <br>_Get the instance attributes of the geometries._  |
|  CInstanceAttributes | [**instances**](classuipc_1_1geometry_1_1_geometry.md#function-instances-22) () const<br> |
|  MetaAttributes | [**meta**](classuipc_1_1geometry_1_1_geometry.md#function-meta-12) () <br>_Get the meta attributes of the geometries._  |
|  CMetaAttributes | [**meta**](classuipc_1_1geometry_1_1_geometry.md#function-meta-22) () const<br> |
|  [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**operator=**](classuipc_1_1geometry_1_1_geometry.md#function-operator) (const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & o) = delete<br> |
|  [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**operator=**](classuipc_1_1geometry_1_1_geometry.md#function-operator_1) ([**Geometry**](classuipc_1_1geometry_1_1_geometry.md) && o) = delete<br> |


## Public Functions inherited from uipc::geometry::IGeometry

See [uipc::geometry::IGeometry](classuipc_1_1geometry_1_1_i_geometry.md)

| Type | Name |
| ---: | :--- |
|  Json | [**to\_json**](classuipc_1_1geometry_1_1_i_geometry.md#function-to_json) () const<br> |
|  std::string\_view | [**type**](classuipc_1_1geometry_1_1_i_geometry.md#function-type) () noexcept const<br>_Get the type of the geometries, check the type to downcast the geometries to a specific type._  |
| virtual  | [**~IGeometry**](classuipc_1_1geometry_1_1_i_geometry.md#function-igeometry) () = default<br> |






















## Protected Attributes inherited from uipc::geometry::Geometry

See [uipc::geometry::Geometry](classuipc_1_1geometry_1_1_geometry.md)

| Type | Name |
| ---: | :--- |
|  [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) | [**m\_intances**](classuipc_1_1geometry_1_1_geometry.md#variable-m_intances)  <br> |
|  [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) | [**m\_meta**](classuipc_1_1geometry_1_1_geometry.md#variable-m_meta)  <br> |














































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_collect\_attribute\_collections**](#function-do_collect_attribute_collections) (vector&lt; std::string &gt; & names, vector&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) override<br> |
| virtual Json | [**do\_to\_json**](#function-do_to_json) () override const<br> |
| virtual std::string\_view | [**get\_type**](#function-get_type) () noexcept override const<br> |


## Protected Functions inherited from uipc::geometry::Geometry

See [uipc::geometry::Geometry](classuipc_1_1geometry_1_1_geometry.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_collect\_attribute\_collections**](classuipc_1_1geometry_1_1_geometry.md#function-do_collect_attribute_collections) (vector&lt; std::string &gt; & names, vector&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) override<br> |
| virtual Json | [**do\_to\_json**](classuipc_1_1geometry_1_1_geometry.md#function-do_to_json) () override const<br> |


## Protected Functions inherited from uipc::geometry::IGeometry

See [uipc::geometry::IGeometry](classuipc_1_1geometry_1_1_i_geometry.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_collect\_attribute\_collections**](classuipc_1_1geometry_1_1_i_geometry.md#function-do_collect_attribute_collections) (vector&lt; std::string &gt; & names, vector&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) = 0<br> |
| virtual Json | [**do\_to\_json**](classuipc_1_1geometry_1_1_i_geometry.md#function-do_to_json) () const = 0<br> |
| virtual std::string\_view | [**get\_type**](classuipc_1_1geometry_1_1_i_geometry.md#function-get_type) () noexcept const = 0<br> |








# Detailed Description


In $\mathbb{R}^3$, a simplicial complex is defined as follows: $$ K = (V, E, F, T), $$ where $V$ is the set of vertices, $E$ is the set of edges, $F$ is the set of triangles, and $T$ is the set of tetrahedra.




**See also:** [Tutorial/Geometry](../tutorial/geometry.md) 



    
## Public Types Documentation




### typedef CEdgeAttributes 

```C++
using uipc::geometry::SimplicialComplex::CEdgeAttributes =  SimplicialComplexAttributes<true, 1>;
```




<hr>



### typedef CTetrahedronAttributes 

```C++
using uipc::geometry::SimplicialComplex::CTetrahedronAttributes =  SimplicialComplexAttributes<true, 3>;
```




<hr>



### typedef CTriangleAttributes 

```C++
using uipc::geometry::SimplicialComplex::CTriangleAttributes =  SimplicialComplexAttributes<true, 2>;
```




<hr>



### typedef CVertexAttributes 

```C++
using uipc::geometry::SimplicialComplex::CVertexAttributes =  SimplicialComplexAttributes<true, 0>;
```




<hr>



### typedef EdgeAttributes 

_Alias for the edge attributes._ 
```C++
using uipc::geometry::SimplicialComplex::EdgeAttributes =  SimplicialComplexAttributes<false, 1>;
```





**See also:** [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) 



        

<hr>



### typedef TetrahedronAttributes 

_Alias for the tetrahedron attributes._ 
```C++
using uipc::geometry::SimplicialComplex::TetrahedronAttributes =  SimplicialComplexAttributes<false, 3>;
```





**See also:** [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) 



        

<hr>



### typedef TriangleAttributes 

_Alias for the triangle attributes._ 
```C++
using uipc::geometry::SimplicialComplex::TriangleAttributes =  SimplicialComplexAttributes<false, 2>;
```





**See also:** [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) 



        

<hr>



### typedef VertexAttributes 

_Alias for the vertex attributes._ 
```C++
using uipc::geometry::SimplicialComplex::VertexAttributes =  SimplicialComplexAttributes<false, 0>;
```





**See also:** [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) 



        

<hr>
## Public Functions Documentation




### function SimplicialComplex [1/3]

```C++
uipc::geometry::SimplicialComplex::SimplicialComplex () 
```




<hr>



### function SimplicialComplex [2/3]

```C++
uipc::geometry::SimplicialComplex::SimplicialComplex (
    const SimplicialComplex & o
) = default
```




<hr>



### function SimplicialComplex [3/3]

```C++
uipc::geometry::SimplicialComplex::SimplicialComplex (
    SimplicialComplex && o
) = default
```




<hr>



### function dim 

_Get the dimension of the simplicial complex._ 
```C++
IndexT uipc::geometry::SimplicialComplex::dim () noexcept const
```



Return the maximum dimension of the simplices in the simplicial complex.




**Returns:**

IndexT 





        

<hr>



### function edges [1/2]

_A wrapper of the edges and its attributes of the simplicial complex._ 
```C++
EdgeAttributes uipc::geometry::SimplicialComplex::edges () noexcept
```





**Returns:**

EdgeAttributes 





        

<hr>



### function edges [2/2]

```C++
CEdgeAttributes uipc::geometry::SimplicialComplex::edges () noexcept const
```




<hr>



### function operator= 

```C++
SimplicialComplex & uipc::geometry::SimplicialComplex::operator= (
    const SimplicialComplex & o
) = delete
```




<hr>



### function operator= 

```C++
SimplicialComplex & uipc::geometry::SimplicialComplex::operator= (
    SimplicialComplex && o
) = delete
```




<hr>



### function positions [1/2]

_Get the positions of the vertices._ 
```C++
AttributeSlot < Vector3 > & uipc::geometry::SimplicialComplex::positions () noexcept
```





**Returns:**

AttributeSlot&lt;Vector3&gt;& 





        

<hr>



### function positions [2/2]

_A short cut to get the positions of the vertices._ 
```C++
const AttributeSlot < Vector3 > & uipc::geometry::SimplicialComplex::positions () noexcept const
```





**Returns:**

const AttributeSlot&lt;Vector3&gt;& 





        

<hr>



### function tetrahedra [1/2]

_A wrapper of the tetrahedra and its attributes of the simplicial complex._ 
```C++
TetrahedronAttributes uipc::geometry::SimplicialComplex::tetrahedra () noexcept
```





**Returns:**

TetrahedronAttributes 





        

<hr>



### function tetrahedra [2/2]

```C++
CTetrahedronAttributes uipc::geometry::SimplicialComplex::tetrahedra () noexcept const
```




<hr>



### function transforms [1/2]

_A short-cut to get the non-const transforms attribute slot._ 
```C++
AttributeSlot < Matrix4x4 > & uipc::geometry::SimplicialComplex::transforms () 
```





**Returns:**

The attribute slot of the non-const transforms. 





        

<hr>



### function transforms [2/2]

_A short-cut to get the const transforms attribute slot._ 
```C++
const AttributeSlot < Matrix4x4 > & uipc::geometry::SimplicialComplex::transforms () const
```





**Returns:**

The attribute slot of the const transforms. 





        

<hr>



### function triangles [1/2]

_A wrapper of the triangles and its attributes of the simplicial complex._ 
```C++
TriangleAttributes uipc::geometry::SimplicialComplex::triangles () noexcept
```





**Returns:**

TriangleAttributes 





        

<hr>



### function triangles [2/2]

```C++
CTriangleAttributes uipc::geometry::SimplicialComplex::triangles () noexcept const
```




<hr>



### function vertices [1/2]

_A wrapper of the vertices and its attributes of the simplicial complex._ 
```C++
VertexAttributes uipc::geometry::SimplicialComplex::vertices () noexcept
```





**Returns:**

VertexAttributeInfo 





        

<hr>



### function vertices [2/2]

```C++
CVertexAttributes uipc::geometry::SimplicialComplex::vertices () noexcept const
```




<hr>
## Protected Functions Documentation




### function do\_collect\_attribute\_collections 

```C++
virtual void uipc::geometry::SimplicialComplex::do_collect_attribute_collections (
    vector< std::string > & names,
    vector< AttributeCollection * > & collections
) override
```



Implements [*uipc::geometry::Geometry::do\_collect\_attribute\_collections*](classuipc_1_1geometry_1_1_geometry.md#function-do_collect_attribute_collections)


<hr>



### function do\_to\_json 

```C++
virtual Json uipc::geometry::SimplicialComplex::do_to_json () override const
```



Implements [*uipc::geometry::Geometry::do\_to\_json*](classuipc_1_1geometry_1_1_geometry.md#function-do_to_json)


<hr>



### function get\_type 

```C++
virtual std::string_view uipc::geometry::SimplicialComplex::get_type () noexcept override const
```



Implements [*uipc::geometry::IGeometry::get\_type*](classuipc_1_1geometry_1_1_i_geometry.md#function-get_type)


<hr>## Friends Documentation





### friend formatter&lt; SimplicialComplex &gt; 

```C++
struct uipc::geometry::SimplicialComplex::formatter< SimplicialComplex > (
    fmt::formatter< SimplicialComplex >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/simplicial_complex.h`

