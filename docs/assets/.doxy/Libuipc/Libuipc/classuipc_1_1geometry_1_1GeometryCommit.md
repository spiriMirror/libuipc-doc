

# Class uipc::geometry::GeometryCommit



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**GeometryCommit**](classuipc_1_1geometry_1_1GeometryCommit.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GeometryCommit**](#function-geometrycommit-14) () = default<br> |
|   | [**GeometryCommit**](#function-geometrycommit-24) (const [**GeometryCommit**](classuipc_1_1geometry_1_1GeometryCommit.md) &) <br> |
|   | [**GeometryCommit**](#function-geometrycommit-34) (const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & dst) <br> |
|  const unordered\_map&lt; std::string, S&lt; [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) &gt; &gt; & | [**attribute\_collections**](#function-attribute_collections) () noexcept const<br> |
|  bool | [**is\_modification**](#function-is_modification) () noexcept const<br> |
|  bool | [**is\_new**](#function-is_new) () noexcept const<br> |
|  bool | [**is\_valid**](#function-is_valid) () noexcept const<br> |
|  S&lt; [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) &gt; | [**new\_geometry**](#function-new_geometry) () noexcept const<br> |
|  [**GeometryCommit**](classuipc_1_1geometry_1_1GeometryCommit.md) & | [**operator=**](#function-operator) (const [**GeometryCommit**](classuipc_1_1geometry_1_1GeometryCommit.md) &) = delete<br> |
|  const std::string & | [**type**](#function-type) () noexcept const<br> |




























## Public Functions Documentation




### function GeometryCommit [1/4]

```C++
uipc::geometry::GeometryCommit::GeometryCommit () = default
```




<hr>



### function GeometryCommit [2/4]

```C++
uipc::geometry::GeometryCommit::GeometryCommit (
    const GeometryCommit &
) 
```




<hr>



### function GeometryCommit [3/4]

```C++
explicit uipc::geometry::GeometryCommit::GeometryCommit (
    const Geometry & dst
) 
```




<hr>



### function attribute\_collections 

```C++
inline const unordered_map< std::string, S< AttributeCollectionCommit > > & uipc::geometry::GeometryCommit::attribute_collections () noexcept const
```




<hr>



### function is\_modification 

```C++
inline bool uipc::geometry::GeometryCommit::is_modification () noexcept const
```




<hr>



### function is\_new 

```C++
inline bool uipc::geometry::GeometryCommit::is_new () noexcept const
```




<hr>



### function is\_valid 

```C++
inline bool uipc::geometry::GeometryCommit::is_valid () noexcept const
```




<hr>



### function new\_geometry 

```C++
inline S< Geometry > uipc::geometry::GeometryCommit::new_geometry () noexcept const
```




<hr>



### function operator= 

```C++
GeometryCommit & uipc::geometry::GeometryCommit::operator= (
    const GeometryCommit &
) = delete
```




<hr>



### function type 

```C++
inline const std::string & uipc::geometry::GeometryCommit::type () noexcept const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry_commit.h`

