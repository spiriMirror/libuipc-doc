

# Class uipc::geometry::GeometryAtlasCommit



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**GeometryAtlasCommit**](classuipc_1_1geometry_1_1GeometryAtlasCommit.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  U&lt; Impl &gt; | [**m\_impl**](#variable-m_impl)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GeometryAtlasCommit**](#function-geometryatlascommit) () <br> |
|  SizeT | [**attribute\_collection\_count**](#function-attribute_collection_count) () noexcept const<br> |
|  vector&lt; std::string &gt; | [**attribute\_collection\_names**](#function-attribute_collection_names) () noexcept const<br> |
|  IndexT | [**create**](#function-create-12) (const [**GeometryCommit**](classuipc_1_1geometry_1_1GeometryCommit.md) & geo\_commit) <br> |
|  void | [**create**](#function-create-22) (std::string\_view name, const [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) & ac\_commit) <br> |
|  S&lt; const [**GeometryCommit**](classuipc_1_1geometry_1_1GeometryCommit.md) &gt; | [**find**](#function-find-12) (IndexT id) const<br> |
|  S&lt; const [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) &gt; | [**find**](#function-find-22) (std::string\_view name) const<br> |
|  void | [**from\_json**](#function-from_json) (const Json & j) <br> |
|  SizeT | [**geometry\_count**](#function-geometry_count) () noexcept const<br> |
|  Json | [**to\_json**](#function-to_json) () const<br> |
|   | [**~GeometryAtlasCommit**](#function-geometryatlascommit) () <br> |




























## Public Attributes Documentation




### variable m\_impl 

```C++
U<Impl> uipc::geometry::GeometryAtlasCommit::m_impl;
```




<hr>
## Public Functions Documentation




### function GeometryAtlasCommit 

```C++
uipc::geometry::GeometryAtlasCommit::GeometryAtlasCommit () 
```




<hr>



### function attribute\_collection\_count 

```C++
SizeT uipc::geometry::GeometryAtlasCommit::attribute_collection_count () noexcept const
```




<hr>



### function attribute\_collection\_names 

```C++
vector< std::string > uipc::geometry::GeometryAtlasCommit::attribute_collection_names () noexcept const
```




<hr>



### function create [1/2]

```C++
IndexT uipc::geometry::GeometryAtlasCommit::create (
    const GeometryCommit & geo_commit
) 
```




<hr>



### function create [2/2]

```C++
void uipc::geometry::GeometryAtlasCommit::create (
    std::string_view name,
    const AttributeCollectionCommit & ac_commit
) 
```




<hr>



### function find [1/2]

```C++
S< const GeometryCommit > uipc::geometry::GeometryAtlasCommit::find (
    IndexT id
) const
```




<hr>



### function find [2/2]

```C++
S< const AttributeCollectionCommit > uipc::geometry::GeometryAtlasCommit::find (
    std::string_view name
) const
```




<hr>



### function from\_json 

```C++
void uipc::geometry::GeometryAtlasCommit::from_json (
    const Json & j
) 
```




<hr>



### function geometry\_count 

```C++
SizeT uipc::geometry::GeometryAtlasCommit::geometry_count () noexcept const
```




<hr>



### function to\_json 

```C++
Json uipc::geometry::GeometryAtlasCommit::to_json () const
```




<hr>



### function ~GeometryAtlasCommit 

```C++
uipc::geometry::GeometryAtlasCommit::~GeometryAtlasCommit () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry_atlas.h`

