

# Class uipc::geometry::GeometryFactory



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**GeometryFactory**](classuipc_1_1geometry_1_1_geometry_factory.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GeometryFactory**](#function-geometryfactory) () <br> |
|  S&lt; [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; | [**create\_slot**](#function-create_slot) (IndexT id, const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & geometry) <br> |
|  vector&lt; S&lt; [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) &gt; &gt; | [**from\_json**](#function-from_json) (const Json & j, span&lt; S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; &gt; attributes) <br> |
|  Json | [**to\_json**](#function-to_json) (span&lt; [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) \* &gt; geos, unordered\_map&lt; [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) \*, IndexT &gt; attr\_to\_index) <br> |
|   | [**~GeometryFactory**](#function-geometryfactory) () <br> |




























## Public Functions Documentation




### function GeometryFactory 

```C++
uipc::geometry::GeometryFactory::GeometryFactory () 
```




<hr>



### function create\_slot 

```C++
S< GeometrySlot > uipc::geometry::GeometryFactory::create_slot (
    IndexT id,
    const Geometry & geometry
) 
```




<hr>



### function from\_json 

```C++
vector< S< Geometry > > uipc::geometry::GeometryFactory::from_json (
    const Json & j,
    span< S< IAttributeSlot > > attributes
) 
```




<hr>



### function to\_json 

```C++
Json uipc::geometry::GeometryFactory::to_json (
    span< Geometry * > geos,
    unordered_map< IAttribute *, IndexT > attr_to_index
) 
```




<hr>



### function ~GeometryFactory 

```C++
uipc::geometry::GeometryFactory::~GeometryFactory () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry_factory.h`

