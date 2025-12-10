

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
|   | [**Geometry**](#function-geometry-23) (const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & o) <br> |
|   | [**Geometry**](#function-geometry-33) ([**Geometry**](classuipc_1_1geometry_1_1_geometry.md) && o) = default<br> |
|  T \* | [**as**](#function-as-12) () <br> |
|  const T \* | [**as**](#function-as-22) () const<br> |
|  [**InstanceAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) | [**instances**](#function-instances-12) () <br>_Get the instance attributes of the geometries._  |
|  [**CInstanceAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) | [**instances**](#function-instances-22) () const<br> |
|  [**MetaAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_meta_attributes_t.md) | [**meta**](#function-meta-12) () <br>_Get the meta attributes of the geometries._  |
|  [**CMetaAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_meta_attributes_t.md) | [**meta**](#function-meta-22) () const<br> |
|  [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**operator=**](#function-operator) (const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & o) = delete<br> |
|  [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**operator=**](#function-operator_1) ([**Geometry**](classuipc_1_1geometry_1_1_geometry.md) && o) = delete<br> |
|  S&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**operator[]**](#function-operator_2) (std::string\_view name) <br>_Get the attribute collection with the given name._  |
|  S&lt; const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**operator[]**](#function-operator_3) (std::string\_view name) const<br>_Get the attribute collection with the given name._  |


## Public Functions inherited from uipc::geometry::IGeometry

See [uipc::geometry::IGeometry](classuipc_1_1geometry_1_1_i_geometry.md)

| Type | Name |
| ---: | :--- |
|  S&lt; [**IGeometry**](classuipc_1_1geometry_1_1_i_geometry.md) &gt; | [**clone**](classuipc_1_1geometry_1_1_i_geometry.md#function-clone) () const<br> |
|  Json | [**to\_json**](classuipc_1_1geometry_1_1_i_geometry.md#function-to_json) () const<br> |
|  std::string\_view | [**type**](classuipc_1_1geometry_1_1_i_geometry.md#function-type) () noexcept const<br>_Get the type of the geometries, check the type to downcast the geometries to a specific type._  |
|  void | [**update\_from**](classuipc_1_1geometry_1_1_i_geometry.md#function-update_from) (const [**GeometryCommit**](classuipc_1_1geometry_1_1_geometry_commit.md) & commit) <br> |
| virtual  | [**~IGeometry**](classuipc_1_1geometry_1_1_i_geometry.md#function-igeometry) () = default<br> |














































## Protected Functions

| Type | Name |
| ---: | :--- |
|  S&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**create**](#function-create) (std::string\_view name) <br>_Create a new attribute collection with the given name._  |
| virtual void | [**do\_build\_from\_attribute\_collections**](#function-do_build_from_attribute_collections) (span&lt; const std::string &gt; names, span&lt; const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; collections) override<br> |
| virtual S&lt; [**IGeometry**](classuipc_1_1geometry_1_1_i_geometry.md) &gt; | [**do\_clone**](#function-do_clone) () override const<br> |
| virtual void | [**do\_collect\_attribute\_collections**](#function-do_collect_attribute_collections-12) (vector&lt; std::string &gt; & names, vector&lt; const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) override const<br> |
| virtual void | [**do\_collect\_attribute\_collections**](#function-do_collect_attribute_collections-22) (vector&lt; std::string &gt; & names, vector&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) override<br> |
| virtual Json | [**do\_to\_json**](#function-do_to_json) () override const<br> |
| virtual void | [**do\_update\_from**](#function-do_update_from) (const [**GeometryCommit**](classuipc_1_1geometry_1_1_geometry_commit.md) & commit) override<br> |
|  S&lt; const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**find**](#function-find-12) (std::string\_view name) const<br>_Find the attribute collection with the given name._  |
|  S&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**find**](#function-find-22) (std::string\_view name) <br> |
| virtual std::string\_view | [**get\_type**](#function-get_type) () noexcept override const<br> |


## Protected Functions inherited from uipc::geometry::IGeometry

See [uipc::geometry::IGeometry](classuipc_1_1geometry_1_1_i_geometry.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_build\_from\_attribute\_collections**](classuipc_1_1geometry_1_1_i_geometry.md#function-do_build_from_attribute_collections) (span&lt; const std::string &gt; names, span&lt; const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; collections) = 0<br> |
| virtual S&lt; [**IGeometry**](classuipc_1_1geometry_1_1_i_geometry.md) &gt; | [**do\_clone**](classuipc_1_1geometry_1_1_i_geometry.md#function-do_clone) () const = 0<br> |
| virtual void | [**do\_collect\_attribute\_collections**](classuipc_1_1geometry_1_1_i_geometry.md#function-do_collect_attribute_collections-12) (vector&lt; std::string &gt; & names, vector&lt; const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) const = 0<br> |
| virtual void | [**do\_collect\_attribute\_collections**](classuipc_1_1geometry_1_1_i_geometry.md#function-do_collect_attribute_collections-22) (vector&lt; std::string &gt; & names, vector&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) = 0<br> |
| virtual Json | [**do\_to\_json**](classuipc_1_1geometry_1_1_i_geometry.md#function-do_to_json) () const = 0<br> |
| virtual void | [**do\_update\_from**](classuipc_1_1geometry_1_1_i_geometry.md#function-do_update_from) (const [**GeometryCommit**](classuipc_1_1geometry_1_1_geometry_commit.md) & commit) = 0<br> |
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
) 
```




<hr>



### function Geometry [3/3]

```C++
uipc::geometry::Geometry::Geometry (
    Geometry && o
) = default
```




<hr>



### function as [1/2]

```C++
template<std::derived_from< Geometry > T>
T * uipc::geometry::Geometry::as () 
```




<hr>



### function as [2/2]

```C++
template<std::derived_from< Geometry > T>
const T * uipc::geometry::Geometry::as () const
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



### function operator[] 

_Get the attribute collection with the given name._ 
```C++
S< AttributeCollection > uipc::geometry::Geometry::operator[] (
    std::string_view name
) 
```



If the attribute collection does not exist, create a new one.




**Parameters:**


* `name` The name of the attribute collection. 



**Returns:**

The attribute collection with the given name. 





        

<hr>



### function operator[] 

_Get the attribute collection with the given name._ 
```C++
S< const AttributeCollection > uipc::geometry::Geometry::operator[] (
    std::string_view name
) const
```



If the attribute collection does not exist, return nullptr.




**Parameters:**


* `name` The name of the attribute collection. 



**Returns:**

The attribute collection with the given name. 





        

<hr>
## Protected Functions Documentation




### function create 

_Create a new attribute collection with the given name._ 
```C++
S< AttributeCollection > uipc::geometry::Geometry::create (
    std::string_view name
) 
```





**Parameters:**


* `name` The name of the attribute collection. 



**Returns:**

The created attribute collection. 





        

<hr>



### function do\_build\_from\_attribute\_collections 

```C++
virtual void uipc::geometry::Geometry::do_build_from_attribute_collections (
    span< const std::string > names,
    span< const AttributeCollection * > collections
) override
```



Implements [*uipc::geometry::IGeometry::do\_build\_from\_attribute\_collections*](classuipc_1_1geometry_1_1_i_geometry.md#function-do_build_from_attribute_collections)


<hr>



### function do\_clone 

```C++
virtual S< IGeometry > uipc::geometry::Geometry::do_clone () override const
```



Implements [*uipc::geometry::IGeometry::do\_clone*](classuipc_1_1geometry_1_1_i_geometry.md#function-do_clone)


<hr>



### function do\_collect\_attribute\_collections [1/2]

```C++
virtual void uipc::geometry::Geometry::do_collect_attribute_collections (
    vector< std::string > & names,
    vector< const AttributeCollection * > & collections
) override const
```



Implements [*uipc::geometry::IGeometry::do\_collect\_attribute\_collections*](classuipc_1_1geometry_1_1_i_geometry.md#function-do_collect_attribute_collections-12)


<hr>



### function do\_collect\_attribute\_collections [2/2]

```C++
virtual void uipc::geometry::Geometry::do_collect_attribute_collections (
    vector< std::string > & names,
    vector< AttributeCollection * > & collections
) override
```



Implements [*uipc::geometry::IGeometry::do\_collect\_attribute\_collections*](classuipc_1_1geometry_1_1_i_geometry.md#function-do_collect_attribute_collections-22)


<hr>



### function do\_to\_json 

```C++
virtual Json uipc::geometry::Geometry::do_to_json () override const
```



Implements [*uipc::geometry::IGeometry::do\_to\_json*](classuipc_1_1geometry_1_1_i_geometry.md#function-do_to_json)


<hr>



### function do\_update\_from 

```C++
virtual void uipc::geometry::Geometry::do_update_from (
    const GeometryCommit & commit
) override
```



Implements [*uipc::geometry::IGeometry::do\_update\_from*](classuipc_1_1geometry_1_1_i_geometry.md#function-do_update_from)


<hr>



### function find [1/2]

_Find the attribute collection with the given name._ 
```C++
S< const AttributeCollection > uipc::geometry::Geometry::find (
    std::string_view name
) const
```





**Parameters:**


* `name` The name of the attribute collection. 



**Returns:**

The attribute collection with the given name. 




**Returns:**

nullptr if the attribute collection with the given name does not exist. 





        

<hr>



### function find [2/2]

```C++
S< AttributeCollection > uipc::geometry::Geometry::find (
    std::string_view name
) 
```




<hr>



### function get\_type 

```C++
virtual std::string_view uipc::geometry::Geometry::get_type () noexcept override const
```



Implements [*uipc::geometry::IGeometry::get\_type*](classuipc_1_1geometry_1_1_i_geometry.md#function-get_type)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry.h`

