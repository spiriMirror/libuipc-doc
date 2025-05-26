

# Class uipc::geometry::AttributeCollectionCommit



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1_attribute_collection_commit.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AttributeCollectionCommit**](#function-attributecollectioncommit-14) () = default<br> |
|   | [**AttributeCollectionCommit**](#function-attributecollectioncommit-24) (const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) & dst) <br> |
|   | [**AttributeCollectionCommit**](#function-attributecollectioncommit-34) (const [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1_attribute_collection_commit.md) & other) = default<br> |
|  const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) & | [**attribute\_collection**](#function-attribute_collection) () noexcept const<br> |
|  [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1_attribute_collection_commit.md) & | [**operator=**](#function-operator) (const [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1_attribute_collection_commit.md) & other) = delete<br> |
|  span&lt; const std::string &gt; | [**removed\_names**](#function-removed_names) () noexcept const<br> |




























## Public Functions Documentation




### function AttributeCollectionCommit [1/4]

```C++
uipc::geometry::AttributeCollectionCommit::AttributeCollectionCommit () = default
```




<hr>



### function AttributeCollectionCommit [2/4]

```C++
explicit uipc::geometry::AttributeCollectionCommit::AttributeCollectionCommit (
    const AttributeCollection & dst
) 
```




<hr>



### function AttributeCollectionCommit [3/4]

```C++
uipc::geometry::AttributeCollectionCommit::AttributeCollectionCommit (
    const AttributeCollectionCommit & other
) = default
```




<hr>



### function attribute\_collection 

```C++
inline const AttributeCollection & uipc::geometry::AttributeCollectionCommit::attribute_collection () noexcept const
```




<hr>



### function operator= 

```C++
AttributeCollectionCommit & uipc::geometry::AttributeCollectionCommit::operator= (
    const AttributeCollectionCommit & other
) = delete
```




<hr>



### function removed\_names 

```C++
inline span< const std::string > uipc::geometry::AttributeCollectionCommit::removed_names () noexcept const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/attribute_collection_commit.h`

