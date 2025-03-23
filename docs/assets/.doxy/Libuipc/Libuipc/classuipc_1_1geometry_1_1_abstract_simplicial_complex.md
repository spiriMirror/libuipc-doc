

# Class uipc::geometry::AbstractSimplicialComplex



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**AbstractSimplicialComplex**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md)



_Represents an abstract simplicial complex, containing vertices, edges, triangles, and tetrahedra._ [More...](#detailed-description)

* `#include <abstract_simplicial_complex.h>`



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
|   | [**AbstractSimplicialComplex**](#function-abstractsimplicialcomplex-13) () = default<br> |
|   | [**AbstractSimplicialComplex**](#function-abstractsimplicialcomplex-23) (const [**AbstractSimplicialComplex**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md) & o) = default<br> |
|   | [**AbstractSimplicialComplex**](#function-abstractsimplicialcomplex-33) ([**AbstractSimplicialComplex**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md) && o) = default<br> |
|  IndexT | [**dim**](#function-dim) () noexcept const<br>_Get the dimension of the simplicial complex._  |
|  [**EdgeAttributes**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md#typedef-edgeattributes) | [**edges**](#function-edges-12) () noexcept<br>_A wrapper of the edges and its attributes of the simplicial complex._  |
|  [**CEdgeAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) | [**edges**](#function-edges-22) () noexcept const<br> |
|  [**AbstractSimplicialComplex**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md) & | [**operator=**](#function-operator) (const [**AbstractSimplicialComplex**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md) & o) = delete<br> |
|  [**AbstractSimplicialComplex**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md) & | [**operator=**](#function-operator_1) ([**AbstractSimplicialComplex**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md) && o) = delete<br> |
|  [**TetrahedronAttributes**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md#typedef-tetrahedronattributes) | [**tetrahedra**](#function-tetrahedra-12) () noexcept<br>_A wrapper of the tetrahedra and its attributes of the simplicial complex._  |
|  [**CTetrahedronAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) | [**tetrahedra**](#function-tetrahedra-22) () noexcept const<br> |
|  [**TriangleAttributes**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md#typedef-triangleattributes) | [**triangles**](#function-triangles-12) () noexcept<br>_A wrapper of the triangles and its attributes of the simplicial complex._  |
|  [**CTriangleAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) | [**triangles**](#function-triangles-22) () noexcept const<br> |
|  [**VertexAttributes**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md#typedef-vertexattributes) | [**vertices**](#function-vertices-12) () noexcept<br>_A wrapper of the vertices and its attributes of the simplicial complex._  |
|  [**CVertexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) | [**vertices**](#function-vertices-22) () noexcept const<br> |


## Public Functions inherited from uipc::geometry::Geometry

See [uipc::geometry::Geometry](classuipc_1_1geometry_1_1_geometry.md)

| Type | Name |
| ---: | :--- |
|   | [**Geometry**](classuipc_1_1geometry_1_1_geometry.md#function-geometry-13) () <br> |
|   | [**Geometry**](classuipc_1_1geometry_1_1_geometry.md#function-geometry-23) (const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & o) = default<br> |
|   | [**Geometry**](classuipc_1_1geometry_1_1_geometry.md#function-geometry-33) ([**Geometry**](classuipc_1_1geometry_1_1_geometry.md) && o) = default<br> |
|  T \* | [**as**](classuipc_1_1geometry_1_1_geometry.md#function-as) () <br> |
|  [**InstanceAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) | [**instances**](classuipc_1_1geometry_1_1_geometry.md#function-instances-12) () <br>_Get the instance attributes of the geometries._  |
|  [**CInstanceAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) | [**instances**](classuipc_1_1geometry_1_1_geometry.md#function-instances-22) () const<br> |
|  [**MetaAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_meta_attributes_t.md) | [**meta**](classuipc_1_1geometry_1_1_geometry.md#function-meta-12) () <br>_Get the meta attributes of the geometries._  |
|  [**CMetaAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_meta_attributes_t.md) | [**meta**](classuipc_1_1geometry_1_1_geometry.md#function-meta-22) () const<br> |
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








## Detailed Description




**Note:**

Abstract simplicial complex does not contain any geometric information, such as coordinates of vertices. 





    
## Public Types Documentation




### typedef CEdgeAttributes 

```C++
using uipc::geometry::AbstractSimplicialComplex::CEdgeAttributes =  SimplicialComplexAttributes<true, 1>;
```




<hr>



### typedef CTetrahedronAttributes 

```C++
using uipc::geometry::AbstractSimplicialComplex::CTetrahedronAttributes =  SimplicialComplexAttributes<true, 3>;
```




<hr>



### typedef CTriangleAttributes 

```C++
using uipc::geometry::AbstractSimplicialComplex::CTriangleAttributes =  SimplicialComplexAttributes<true, 2>;
```




<hr>



### typedef CVertexAttributes 

```C++
using uipc::geometry::AbstractSimplicialComplex::CVertexAttributes =  SimplicialComplexAttributes<true, 0>;
```




<hr>



### typedef EdgeAttributes 

_Alias for the edge attributes._ 
```C++
using uipc::geometry::AbstractSimplicialComplex::EdgeAttributes =  SimplicialComplexAttributes<false, 1>;
```





**See also:** [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) 



        

<hr>



### typedef TetrahedronAttributes 

_Alias for the tetrahedron attributes._ 
```C++
using uipc::geometry::AbstractSimplicialComplex::TetrahedronAttributes =  SimplicialComplexAttributes<false, 3>;
```





**See also:** [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) 



        

<hr>



### typedef TriangleAttributes 

_Alias for the triangle attributes._ 
```C++
using uipc::geometry::AbstractSimplicialComplex::TriangleAttributes =  SimplicialComplexAttributes<false, 2>;
```





**See also:** [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) 



        

<hr>



### typedef VertexAttributes 

_Alias for the vertex attributes._ 
```C++
using uipc::geometry::AbstractSimplicialComplex::VertexAttributes =  SimplicialComplexAttributes<false, 0>;
```





**See also:** [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) 



        

<hr>
## Public Functions Documentation




### function AbstractSimplicialComplex [1/3]

```C++
uipc::geometry::AbstractSimplicialComplex::AbstractSimplicialComplex () = default
```




<hr>



### function AbstractSimplicialComplex [2/3]

```C++
uipc::geometry::AbstractSimplicialComplex::AbstractSimplicialComplex (
    const AbstractSimplicialComplex & o
) = default
```




<hr>



### function AbstractSimplicialComplex [3/3]

```C++
uipc::geometry::AbstractSimplicialComplex::AbstractSimplicialComplex (
    AbstractSimplicialComplex && o
) = default
```




<hr>



### function dim 

_Get the dimension of the simplicial complex._ 
```C++
IndexT uipc::geometry::AbstractSimplicialComplex::dim () noexcept const
```



Return the maximum dimension of the simplices in the simplicial complex.




**Returns:**

IndexT 





        

<hr>



### function edges [1/2]

_A wrapper of the edges and its attributes of the simplicial complex._ 
```C++
EdgeAttributes uipc::geometry::AbstractSimplicialComplex::edges () noexcept
```





**Returns:**

[**EdgeAttributes**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md#typedef-edgeattributes) 





        

<hr>



### function edges [2/2]

```C++
CEdgeAttributes uipc::geometry::AbstractSimplicialComplex::edges () noexcept const
```




<hr>



### function operator= 

```C++
AbstractSimplicialComplex & uipc::geometry::AbstractSimplicialComplex::operator= (
    const AbstractSimplicialComplex & o
) = delete
```




<hr>



### function operator= 

```C++
AbstractSimplicialComplex & uipc::geometry::AbstractSimplicialComplex::operator= (
    AbstractSimplicialComplex && o
) = delete
```




<hr>



### function tetrahedra [1/2]

_A wrapper of the tetrahedra and its attributes of the simplicial complex._ 
```C++
TetrahedronAttributes uipc::geometry::AbstractSimplicialComplex::tetrahedra () noexcept
```





**Returns:**

[**TetrahedronAttributes**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md#typedef-tetrahedronattributes) 





        

<hr>



### function tetrahedra [2/2]

```C++
CTetrahedronAttributes uipc::geometry::AbstractSimplicialComplex::tetrahedra () noexcept const
```




<hr>



### function triangles [1/2]

_A wrapper of the triangles and its attributes of the simplicial complex._ 
```C++
TriangleAttributes uipc::geometry::AbstractSimplicialComplex::triangles () noexcept
```





**Returns:**

[**TriangleAttributes**](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md#typedef-triangleattributes) 





        

<hr>



### function triangles [2/2]

```C++
CTriangleAttributes uipc::geometry::AbstractSimplicialComplex::triangles () noexcept const
```




<hr>



### function vertices [1/2]

_A wrapper of the vertices and its attributes of the simplicial complex._ 
```C++
VertexAttributes uipc::geometry::AbstractSimplicialComplex::vertices () noexcept
```





**Returns:**

VertexAttributeInfo 





        

<hr>



### function vertices [2/2]

```C++
CVertexAttributes uipc::geometry::AbstractSimplicialComplex::vertices () noexcept const
```




<hr>
## Protected Functions Documentation




### function do\_to\_json 

```C++
virtual Json uipc::geometry::AbstractSimplicialComplex::do_to_json () override const
```



Implements [*uipc::geometry::Geometry::do\_to\_json*](classuipc_1_1geometry_1_1_geometry.md#function-do_to_json)


<hr>



### function get\_type 

```C++
virtual std::string_view uipc::geometry::AbstractSimplicialComplex::get_type () noexcept override const
```



Implements [*uipc::geometry::IGeometry::get\_type*](classuipc_1_1geometry_1_1_i_geometry.md#function-get_type)


<hr>## Friends Documentation





### friend formatter&lt; AbstractSimplicialComplex &gt; 

```C++
struct uipc::geometry::AbstractSimplicialComplex::formatter< AbstractSimplicialComplex > (
    fmt::formatter< AbstractSimplicialComplex >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/abstract_simplicial_complex.h`

