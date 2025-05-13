

# Class uipc::geometry::GeometryAtlas



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**GeometryAtlas**](classuipc_1_1geometry_1_1_geometry_atlas.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GeometryAtlas**](#function-geometryatlas) () <br> |
|  SizeT | [**attribute\_collection\_count**](#function-attribute_collection_count) () noexcept const<br> |
|  vector&lt; std::string &gt; | [**attribute\_collection\_names**](#function-attribute_collection_names) () noexcept const<br> |
|  IndexT | [**create**](#function-create-12) (const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & geo) <br>_Create a geometry in the atlas._  |
|  void | [**create**](#function-create-22) (std::string\_view name, const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) & ac) <br>_Create a named_ [_**AttributeCollection**_](classuipc_1_1geometry_1_1_attribute_collection.md) _in the atlas._ |
|  const [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) \* | [**find**](#function-find-12) (IndexT id) const<br>_Find the geometry slot by id._  |
|  const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* | [**find**](#function-find-22) (std::string\_view name) const<br>_Find the_ [_**AttributeCollection**_](classuipc_1_1geometry_1_1_attribute_collection.md) _by name._ |
|  void | [**from\_json**](#function-from_json) (const Json & j) <br>_Create geometry atlas from json._  |
|  SizeT | [**geometry\_count**](#function-geometry_count) () noexcept const<br> |
|  Json | [**to\_json**](#function-to_json) () const<br>_Create json representation of the geometry atlas._  |
|   | [**~GeometryAtlas**](#function-geometryatlas) () <br> |




























## Public Functions Documentation




### function GeometryAtlas 

```C++
uipc::geometry::GeometryAtlas::GeometryAtlas () 
```




<hr>



### function attribute\_collection\_count 

```C++
SizeT uipc::geometry::GeometryAtlas::attribute_collection_count () noexcept const
```




<hr>



### function attribute\_collection\_names 

```C++
vector< std::string > uipc::geometry::GeometryAtlas::attribute_collection_names () noexcept const
```




<hr>



### function create [1/2]

```C++
IndexT uipc::geometry::GeometryAtlas::create (
    const Geometry & geo
) 
```




<hr>



### function create [2/2]

```C++
void uipc::geometry::GeometryAtlas::create (
    std::string_view name,
    const AttributeCollection & ac
) 
```




<hr>



### function find [1/2]

_Find the geometry slot by id._ 
```C++
const GeometrySlot * uipc::geometry::GeometryAtlas::find (
    IndexT id
) const
```



Only return const version, not allow to modify the geometry. 


        

<hr>



### function find [2/2]

_Find the_ [_**AttributeCollection**_](classuipc_1_1geometry_1_1_attribute_collection.md) _by name._
```C++
const AttributeCollection * uipc::geometry::GeometryAtlas::find (
    std::string_view name
) const
```



Only return const version, not allow to modify the geometry. 


        

<hr>



### function from\_json 

_Create geometry atlas from json._ 
```C++
void uipc::geometry::GeometryAtlas::from_json (
    const Json & j
) 
```





**Parameters:**


* `j` The json representation of the geometry atlas 
* `attributes` The attributes to be used in the geometry 




        

<hr>



### function geometry\_count 

```C++
SizeT uipc::geometry::GeometryAtlas::geometry_count () noexcept const
```




<hr>



### function to\_json 

```C++
Json uipc::geometry::GeometryAtlas::to_json () const
```




<hr>



### function ~GeometryAtlas 

```C++
uipc::geometry::GeometryAtlas::~GeometryAtlas () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry_atlas.h`

