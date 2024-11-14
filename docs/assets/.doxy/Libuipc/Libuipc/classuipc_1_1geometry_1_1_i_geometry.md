

# Class uipc::geometry::IGeometry



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**IGeometry**](classuipc_1_1geometry_1_1_i_geometry.md)



_An abstract class for geometries._ 

* `#include <geometry.h>`





Inherited by the following classes: [uipc::geometry::Geometry](classuipc_1_1geometry_1_1_geometry.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  Json | [**to\_json**](#function-to_json) () const<br> |
|  std::string\_view | [**type**](#function-type) () noexcept const<br>_Get the type of the geometries, check the type to downcast the geometries to a specific type._  |
| virtual  | [**~IGeometry**](#function-igeometry) () = default<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_collect\_attribute\_collections**](#function-do_collect_attribute_collections) (vector&lt; std::string &gt; & names, vector&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) = 0<br> |
| virtual Json | [**do\_to\_json**](#function-do_to_json) () const = 0<br> |
| virtual std::string\_view | [**get\_type**](#function-get_type) () noexcept const = 0<br> |




## Public Functions Documentation




### function to\_json 

```C++
Json uipc::geometry::IGeometry::to_json () const
```




<hr>



### function type 

_Get the type of the geometries, check the type to downcast the geometries to a specific type._ 
```C++
std::string_view uipc::geometry::IGeometry::type () noexcept const
```





**Returns:**

a string\_view of the type of the geometries 





        

<hr>



### function ~IGeometry 

```C++
virtual uipc::geometry::IGeometry::~IGeometry () = default
```




<hr>
## Protected Functions Documentation




### function do\_collect\_attribute\_collections 

```C++
virtual void uipc::geometry::IGeometry::do_collect_attribute_collections (
    vector< std::string > & names,
    vector< AttributeCollection * > & collections
) = 0
```




<hr>



### function do\_to\_json 

```C++
virtual Json uipc::geometry::IGeometry::do_to_json () const = 0
```




<hr>



### function get\_type 

```C++
virtual std::string_view uipc::geometry::IGeometry::get_type () noexcept const = 0
```




<hr>## Friends Documentation





### friend GeometryVisitor 

```C++
class uipc::geometry::IGeometry::GeometryVisitor (
    backend::GeometryVisitor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry.h`

