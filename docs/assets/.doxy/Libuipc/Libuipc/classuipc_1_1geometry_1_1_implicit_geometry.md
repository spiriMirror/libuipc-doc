

# Class uipc::geometry::ImplicitGeometry



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**ImplicitGeometry**](classuipc_1_1geometry_1_1_implicit_geometry.md)








Inherits the following classes: [uipc::geometry::Geometry](classuipc_1_1geometry_1_1_geometry.md)
















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
|   | [**ImplicitGeometry**](#function-implicitgeometry) () <br> |
|  std::string\_view | [**name**](#function-name) () noexcept const<br> |
|  const [**builtin::UIDInfo**](structuipc_1_1builtin_1_1_u_i_d_info.md) & | [**uid\_info**](#function-uid_info) () noexcept const<br> |


## Public Functions inherited from uipc::geometry::Geometry

See [uipc::geometry::Geometry](classuipc_1_1geometry_1_1_geometry.md)

| Type | Name |
| ---: | :--- |
|   | [**Geometry**](classuipc_1_1geometry_1_1_geometry.md#function-geometry-13) () <br> |
|   | [**Geometry**](classuipc_1_1geometry_1_1_geometry.md#function-geometry-23) (const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & o) <br> |
|   | [**Geometry**](classuipc_1_1geometry_1_1_geometry.md#function-geometry-33) ([**Geometry**](classuipc_1_1geometry_1_1_geometry.md) && o) = default<br> |
|  T \* | [**as**](classuipc_1_1geometry_1_1_geometry.md#function-as-12) () <br> |
|  const T \* | [**as**](classuipc_1_1geometry_1_1_geometry.md#function-as-22) () const<br> |
|  [**InstanceAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) | [**instances**](classuipc_1_1geometry_1_1_geometry.md#function-instances-12) () <br>_Get the instance attributes of the geometries._  |
|  [**CInstanceAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_instance_attributes_t.md) | [**instances**](classuipc_1_1geometry_1_1_geometry.md#function-instances-22) () const<br> |
|  [**MetaAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_meta_attributes_t.md) | [**meta**](classuipc_1_1geometry_1_1_geometry.md#function-meta-12) () <br>_Get the meta attributes of the geometries._  |
|  [**CMetaAttributes**](classuipc_1_1geometry_1_1_geometry_1_1_meta_attributes_t.md) | [**meta**](classuipc_1_1geometry_1_1_geometry.md#function-meta-22) () const<br> |
|  [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**operator=**](classuipc_1_1geometry_1_1_geometry.md#function-operator) (const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & o) = delete<br> |
|  [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**operator=**](classuipc_1_1geometry_1_1_geometry.md#function-operator_1) ([**Geometry**](classuipc_1_1geometry_1_1_geometry.md) && o) = delete<br> |
|  S&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**operator[]**](classuipc_1_1geometry_1_1_geometry.md#function-operator_2) (std::string\_view name) <br>_Get the attribute collection with the given name._  |
|  S&lt; const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**operator[]**](classuipc_1_1geometry_1_1_geometry.md#function-operator_3) (std::string\_view name) const<br>_Get the attribute collection with the given name._  |


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
| virtual S&lt; [**IGeometry**](classuipc_1_1geometry_1_1_i_geometry.md) &gt; | [**do\_clone**](#function-do_clone) () override const<br> |
| virtual std::string\_view | [**get\_type**](#function-get_type) () noexcept override const<br> |


## Protected Functions inherited from uipc::geometry::Geometry

See [uipc::geometry::Geometry](classuipc_1_1geometry_1_1_geometry.md)

| Type | Name |
| ---: | :--- |
|  S&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**create**](classuipc_1_1geometry_1_1_geometry.md#function-create) (std::string\_view name) <br>_Create a new attribute collection with the given name._  |
| virtual void | [**do\_build\_from\_attribute\_collections**](classuipc_1_1geometry_1_1_geometry.md#function-do_build_from_attribute_collections) (span&lt; const std::string &gt; names, span&lt; const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; collections) override<br> |
| virtual S&lt; [**IGeometry**](classuipc_1_1geometry_1_1_i_geometry.md) &gt; | [**do\_clone**](classuipc_1_1geometry_1_1_geometry.md#function-do_clone) () override const<br> |
| virtual void | [**do\_collect\_attribute\_collections**](classuipc_1_1geometry_1_1_geometry.md#function-do_collect_attribute_collections-12) (vector&lt; std::string &gt; & names, vector&lt; const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) override const<br> |
| virtual void | [**do\_collect\_attribute\_collections**](classuipc_1_1geometry_1_1_geometry.md#function-do_collect_attribute_collections-22) (vector&lt; std::string &gt; & names, vector&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* &gt; & collections) override<br> |
| virtual Json | [**do\_to\_json**](classuipc_1_1geometry_1_1_geometry.md#function-do_to_json) () override const<br> |
| virtual void | [**do\_update\_from**](classuipc_1_1geometry_1_1_geometry.md#function-do_update_from) (const [**GeometryCommit**](classuipc_1_1geometry_1_1_geometry_commit.md) & commit) override<br> |
|  S&lt; const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**find**](classuipc_1_1geometry_1_1_geometry.md#function-find-12) (std::string\_view name) const<br>_Find the attribute collection with the given name._  |
|  S&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**find**](classuipc_1_1geometry_1_1_geometry.md#function-find-22) (std::string\_view name) <br> |
| virtual std::string\_view | [**get\_type**](classuipc_1_1geometry_1_1_geometry.md#function-get_type) () noexcept override const<br> |


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








## Public Functions Documentation




### function ImplicitGeometry 

```C++
uipc::geometry::ImplicitGeometry::ImplicitGeometry () 
```




<hr>



### function name 

```C++
std::string_view uipc::geometry::ImplicitGeometry::name () noexcept const
```




<hr>



### function uid\_info 

```C++
const builtin::UIDInfo & uipc::geometry::ImplicitGeometry::uid_info () noexcept const
```




<hr>
## Protected Functions Documentation




### function do\_clone 

```C++
virtual S< IGeometry > uipc::geometry::ImplicitGeometry::do_clone () override const
```



Implements [*uipc::geometry::Geometry::do\_clone*](classuipc_1_1geometry_1_1_geometry.md#function-do_clone)


<hr>



### function get\_type 

```C++
virtual std::string_view uipc::geometry::ImplicitGeometry::get_type () noexcept override const
```



Implements [*uipc::geometry::Geometry::get\_type*](classuipc_1_1geometry_1_1_geometry.md#function-get_type)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/implicit_geometry.h`

