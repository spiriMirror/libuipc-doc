

# Class uipc::geometry::GeometryAtlas



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**GeometryAtlas**](classuipc_1_1geometry_1_1GeometryAtlas.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GeometryAtlas**](#function-geometryatlas) () <br> |
|  SizeT | [**attribute\_collection\_count**](#function-attribute_collection_count) () noexcept const<br> |
|  vector&lt; std::string &gt; | [**attribute\_collection\_names**](#function-attribute_collection_names) () noexcept const<br> |
|  IndexT | [**create**](#function-create-12) (const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & geo, bool evolving\_only=false) <br>_Create a geometry in the atlas._  |
|  void | [**create**](#function-create-22) (std::string\_view name, const [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) & ac, bool evolving\_only=false) <br>_Create a named_ [_**AttributeCollection**_](classuipc_1_1geometry_1_1AttributeCollection.md) _in the atlas._ |
|  S&lt; const [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &gt; | [**find**](#function-find-12) (IndexT id) const<br>_Find the geometry slot by id._  |
|  S&lt; const [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) &gt; | [**find**](#function-find-22) (std::string\_view name) const<br>_Find the_ [_**AttributeCollection**_](classuipc_1_1geometry_1_1AttributeCollection.md) _by name._ |
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

_Create a geometry in the atlas._ 
```C++
IndexT uipc::geometry::GeometryAtlas::create (
    const Geometry & geo,
    bool evolving_only=false
) 
```




<hr>



### function create [2/2]

_Create a named_ [_**AttributeCollection**_](classuipc_1_1geometry_1_1AttributeCollection.md) _in the atlas._
```C++
void uipc::geometry::GeometryAtlas::create (
    std::string_view name,
    const AttributeCollection & ac,
    bool evolving_only=false
) 
```




<hr>



### function find [1/2]

_Find the geometry slot by id._ 
```C++
S< const GeometrySlot > uipc::geometry::GeometryAtlas::find (
    IndexT id
) const
```



Only return const version, not allow to modify the geometry. 


        

<hr>



### function find [2/2]

_Find the_ [_**AttributeCollection**_](classuipc_1_1geometry_1_1AttributeCollection.md) _by name._
```C++
S< const AttributeCollection > uipc::geometry::GeometryAtlas::find (
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

_Create json representation of the geometry atlas._ 
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

