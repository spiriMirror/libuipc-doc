

# Class uipc::core::Object::Geometries



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**Object**](classuipc_1_1core_1_1_object.md) **>** [**Geometries**](classuipc_1_1core_1_1_object_1_1_geometries.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**ObjectGeometrySlots**](classuipc_1_1core_1_1_object_geometry_slots.md)&lt; GeometryT &gt; | [**create**](#function-create-12) (const GeometryT & geometry) <br> |
|  [**ObjectGeometrySlots**](classuipc_1_1core_1_1_object_geometry_slots.md)&lt; GeometryT &gt; | [**create**](#function-create-22) (const GeometryT & geometry, const GeometryT & rest\_geometry) <br> |
|  span&lt; const IndexT &gt; | [**ids**](#function-ids) () noexcept<br> |




























## Public Functions Documentation




### function create [1/2]

```C++
template<std::derived_from< geometry::Geometry > GeometryT>
ObjectGeometrySlots < GeometryT > uipc::core::Object::Geometries::create (
    const GeometryT & geometry
) 
```




<hr>



### function create [2/2]

```C++
template<std::derived_from< geometry::Geometry > GeometryT>
ObjectGeometrySlots < GeometryT > uipc::core::Object::Geometries::create (
    const GeometryT & geometry,
    const GeometryT & rest_geometry
) 
```




<hr>



### function ids 

```C++
span< const IndexT > uipc::core::Object::Geometries::ids () noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/object.h`

