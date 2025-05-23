

# Class uipc::geometry::GeometryFactory



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**GeometryFactory**](classuipc_1_1geometry_1_1_geometry_factory.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GeometryFactory**](#function-geometryfactory) () <br> |
|  S&lt; [**GeometryCommit**](classuipc_1_1geometry_1_1_geometry_commit.md) &gt; | [**commit\_from\_json**](#function-commit_from_json) (const Json & j, [**DeserialSharedAttributeContext**](classuipc_1_1geometry_1_1_deserial_shared_attribute_context.md) & ctx) <br> |
|  Json | [**commit\_to\_json**](#function-commit_to_json) (const [**GeometryCommit**](classuipc_1_1geometry_1_1_geometry_commit.md) & gc, [**SerialSharedAttributeContext**](classuipc_1_1geometry_1_1_serial_shared_attribute_context.md) & ctx) <br> |
|  S&lt; [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; | [**create\_slot**](#function-create_slot) (IndexT id, const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & geometry) <br> |
|  vector&lt; S&lt; [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) &gt; &gt; | [**from\_json**](#function-from_json) (const Json & j, [**DeserialSharedAttributeContext**](classuipc_1_1geometry_1_1_deserial_shared_attribute_context.md) & ctx) <br> |
|  Json | [**to\_json**](#function-to_json-12) (span&lt; [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) \* &gt; geos, [**SerialSharedAttributeContext**](classuipc_1_1geometry_1_1_serial_shared_attribute_context.md) & ctx) <br> |
|  Json | [**to\_json**](#function-to_json-22) ([**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & geos, [**SerialSharedAttributeContext**](classuipc_1_1geometry_1_1_serial_shared_attribute_context.md) & ctx) <br> |
|   | [**~GeometryFactory**](#function-geometryfactory) () <br> |




























## Public Functions Documentation




### function GeometryFactory 

```C++
uipc::geometry::GeometryFactory::GeometryFactory () 
```




<hr>



### function commit\_from\_json 

```C++
S< GeometryCommit > uipc::geometry::GeometryFactory::commit_from_json (
    const Json & j,
    DeserialSharedAttributeContext & ctx
) 
```




<hr>



### function commit\_to\_json 

```C++
Json uipc::geometry::GeometryFactory::commit_to_json (
    const GeometryCommit & gc,
    SerialSharedAttributeContext & ctx
) 
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
    DeserialSharedAttributeContext & ctx
) 
```




<hr>



### function to\_json [1/2]

```C++
Json uipc::geometry::GeometryFactory::to_json (
    span< Geometry * > geos,
    SerialSharedAttributeContext & ctx
) 
```




<hr>



### function to\_json [2/2]

```C++
Json uipc::geometry::GeometryFactory::to_json (
    Geometry & geos,
    SerialSharedAttributeContext & ctx
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

