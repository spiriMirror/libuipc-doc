

# Class uipc::geometry::Geometry



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**Geometry**](classuipc_1_1geometry_1_1_geometry.md)



_A base geometries class that contains the instance attributes and the meta attributes._ 

* `#include <geometry.h>`



Inherits the following classes: [uipc::geometry::IGeometry](classuipc_1_1geometry_1_1_i_geometry.md)


Inherited by the following classes: [uipc::geometry::AbstractSimplicialComplex](classuipc_1_1geometry_1_1_abstract_simplicial_complex.md),  [uipc::geometry::ImplicitGeometry](classuipc_1_1geometry_1_1_implicit_geometry.md),  [uipc::geometry::SimplicialComplex](classuipc_1_1geometry_1_1_simplicial_complex.md)










## Classes

| Type | Name |
| ---: | :--- |
| class | [**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) &lt;IsConst&gt;<br>_A wrapper class for the instance attributes of a geometries._  |
| class | [**MetaAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_meta_attributes_t.md) &lt;IsConst&gt;<br>_A wrapper class for the meta attributes of a geometries._  |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md)&lt; true &gt; | [**CInstanceAttributes**](#typedef-cinstanceattributes)  <br> |
| typedef [**MetaAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_meta_attributes_t.md)&lt; true &gt; | [**CMetaAttributes**](#typedef-cmetaattributes)  <br> |
| typedef [**InstanceAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md)&lt; false &gt; | [**InstanceAttributes**](#typedef-instanceattributes)  <br> |
| typedef [**MetaAttributesT**](classuipc_1_1geometry_1_1_geometry_1_1_meta_attributes_t.md)&lt; false &gt; | [**MetaAttributes**](#typedef-metaattributes)  <br> |








































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Geometry**](#function-geometry-13) () <br> |
|   | [**Geometry**](#function-geometry-23) (const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & o) = default<br> |
|   | [**Geometry**](#function-geometry-33) ([**Geometry**](classuipc_1_1geometry_1_1_geometry.md) && o) = default<br> |
|  T \* | [**as**](#function-as) () <br> |
|  InstanceAttributes | [**instances**](#function-instances-12) () <br>_Get the instance attributes of the geometries._  |
|  CInstanceAttributes | [**instances**](#function-instances-22) () const<br> |
|  MetaAttributes | [**meta**](#function-meta-12) () <br>_Get the meta attributes of the geometries._  |
|  CMetaAttributes | [**meta**](#function-meta-22) () const<br> |
|  [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**operator=**](#function-operator) (const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & o) = delete<br> |
|  [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**operator=**](#function-operator_1) ([**Geometry**](classuipc_1_1geometry_1_1_geometry.md) && o) = delete<br> |


## Public Functions inherited from uipc::geometry::IGeometry

See [uipc::geometry::IGeometry](classuipc_1_1geometry_1_1_i_geometry.md)

| Type | Name |
| ---: | :--- |
|  Json | [**to\_json**](classuipc_1_1geometry_1_1_i_geometry.md#function-to_json) () const<br> |
|  std::string\_view | [**type**](classuipc_1_1geometry_1_1_i_geometry.md#function-type) () noexcept const<br>_Get the type of the geometries, check the type to downcast the geometries to a specific type._  |
| virtual  | [**~IGeometry**](classuipc_1_1geometry_1_1_i_geometry.md#function-igeometry) () = default<br> |














## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) | [**m\_intances**](#variable-m_intances)  <br> |
|  [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) | [**m\_meta**](#variable-m_meta)  <br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_collect\_attribute\_collections**](#function-do_collect_attribute_collections) (vector&lt; std::string &gt; & names, vector&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) override<br> |
| virtual Json | [**do\_to\_json**](#function-do_to_json) () override const<br> |


## Protected Functions inherited from uipc::geometry::IGeometry

See [uipc::geometry::IGeometry](classuipc_1_1geometry_1_1_i_geometry.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_collect\_attribute\_collections**](classuipc_1_1geometry_1_1_i_geometry.md#function-do_collect_attribute_collections) (vector&lt; std::string &gt; & names, vector&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) = 0<br> |
| virtual Json | [**do\_to\_json**](classuipc_1_1geometry_1_1_i_geometry.md#function-do_to_json) () const = 0<br> |
| virtual std::string\_view | [**get\_type**](classuipc_1_1geometry_1_1_i_geometry.md#function-get_type) () noexcept const = 0<br> |






## Public Types Documentation




### typedef CInstanceAttributes 

```C++
using uipc::geometry::Geometry::CInstanceAttributes =  InstanceAttributesT<true>;
```




<hr>



### typedef CMetaAttributes 

```C++
using uipc::geometry::Geometry::CMetaAttributes =  MetaAttributesT<true>;
```




<hr>



### typedef InstanceAttributes 

```C++
using uipc::geometry::Geometry::InstanceAttributes =  InstanceAttributesT<false>;
```




<hr>



### typedef MetaAttributes 

```C++
using uipc::geometry::Geometry::MetaAttributes =  MetaAttributesT<false>;
```




<hr>
## Public Functions Documentation




### function Geometry [1/3]

```C++
uipc::geometry::Geometry::Geometry () 
```




<hr>



### function Geometry [2/3]

```C++
uipc::geometry::Geometry::Geometry (
    const Geometry & o
) = default
```




<hr>



### function Geometry [3/3]

```C++
uipc::geometry::Geometry::Geometry (
    Geometry && o
) = default
```




<hr>



### function as 

```C++
template<std::derived_from< Geometry > T>
T * uipc::geometry::Geometry::as () 
```




<hr>



### function instances [1/2]

_Get the instance attributes of the geometries._ 
```C++
InstanceAttributes uipc::geometry::Geometry::instances () 
```





**Returns:**

The instance attributes of the geometries. 





        

<hr>



### function instances [2/2]

```C++
CInstanceAttributes uipc::geometry::Geometry::instances () const
```




<hr>



### function meta [1/2]

_Get the meta attributes of the geometries._ 
```C++
MetaAttributes uipc::geometry::Geometry::meta () 
```





**Returns:**

The meta attributes of the geometries. 





        

<hr>



### function meta [2/2]

```C++
CMetaAttributes uipc::geometry::Geometry::meta () const
```




<hr>



### function operator= 

```C++
Geometry & uipc::geometry::Geometry::operator= (
    const Geometry & o
) = delete
```




<hr>



### function operator= 

```C++
Geometry & uipc::geometry::Geometry::operator= (
    Geometry && o
) = delete
```




<hr>
## Protected Attributes Documentation




### variable m\_intances 

```C++
AttributeCollection uipc::geometry::Geometry::m_intances;
```




<hr>



### variable m\_meta 

```C++
AttributeCollection uipc::geometry::Geometry::m_meta;
```




<hr>
## Protected Functions Documentation




### function do\_collect\_attribute\_collections 

```C++
virtual void uipc::geometry::Geometry::do_collect_attribute_collections (
    vector< std::string > & names,
    vector< AttributeCollection * > & collections
) override
```



Implements [*uipc::geometry::IGeometry::do\_collect\_attribute\_collections*](classuipc_1_1geometry_1_1_i_geometry.md#function-do_collect_attribute_collections)


<hr>



### function do\_to\_json 

```C++
virtual Json uipc::geometry::Geometry::do_to_json () override const
```



Implements [*uipc::geometry::IGeometry::do\_to\_json*](classuipc_1_1geometry_1_1_i_geometry.md#function-do_to_json)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry.h`

