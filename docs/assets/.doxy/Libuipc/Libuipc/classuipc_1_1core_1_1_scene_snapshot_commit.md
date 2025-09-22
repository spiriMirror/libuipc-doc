

# Class uipc::core::SceneSnapshotCommit



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SceneSnapshotCommit**](classuipc_1_1core_1_1_scene_snapshot_commit.md)



[More...](#detailed-description)

* `#include <scene_snapshot.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SceneSnapshotCommit**](#function-scenesnapshotcommit-12) () = default<br> |
|   | [**SceneSnapshotCommit**](#function-scenesnapshotcommit-22) (const [**SceneSnapshot**](classuipc_1_1core_1_1_scene_snapshot.md) & dst, const [**SceneSnapshot**](classuipc_1_1core_1_1_scene_snapshot.md) & src) <br> |
|  const [**geometry::AttributeCollectionCommit**](classuipc_1_1geometry_1_1_attribute_collection_commit.md) & | [**config**](#function-config) () noexcept const<br> |
|  const vector&lt; [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) &gt; & | [**contact\_elements**](#function-contact_elements) () noexcept const<br> |
|  const [**geometry::AttributeCollectionCommit**](classuipc_1_1geometry_1_1_attribute_collection_commit.md) & | [**contact\_models**](#function-contact_models) () noexcept const<br> |
|  const unordered\_map&lt; IndexT, S&lt; [**geometry::GeometryCommit**](classuipc_1_1geometry_1_1_geometry_commit.md) &gt; &gt; & | [**geometries**](#function-geometries) () noexcept const<br> |
|  bool | [**is\_valid**](#function-is_valid) () noexcept const<br> |
|  const [**ObjectCollectionSnapshot**](classuipc_1_1core_1_1_object_collection_snapshot.md) & | [**object\_collection**](#function-object_collection) () noexcept const<br> |
|  const unordered\_map&lt; IndexT, S&lt; [**geometry::GeometryCommit**](classuipc_1_1geometry_1_1_geometry_commit.md) &gt; &gt; & | [**rest\_geometries**](#function-rest_geometries) () noexcept const<br> |




























## Detailed Description


SceneSnapCommit (from B to A) = SceneSnapshotA - SceneSnapshotB 


    
## Public Functions Documentation




### function SceneSnapshotCommit [1/2]

```C++
uipc::core::SceneSnapshotCommit::SceneSnapshotCommit () = default
```




<hr>



### function SceneSnapshotCommit [2/2]

```C++
uipc::core::SceneSnapshotCommit::SceneSnapshotCommit (
    const SceneSnapshot & dst,
    const SceneSnapshot & src
) 
```




<hr>



### function config 

```C++
inline const geometry::AttributeCollectionCommit & uipc::core::SceneSnapshotCommit::config () noexcept const
```




<hr>



### function contact\_elements 

```C++
inline const vector< ContactElement > & uipc::core::SceneSnapshotCommit::contact_elements () noexcept const
```




<hr>



### function contact\_models 

```C++
inline const geometry::AttributeCollectionCommit & uipc::core::SceneSnapshotCommit::contact_models () noexcept const
```




<hr>



### function geometries 

```C++
inline const unordered_map< IndexT, S< geometry::GeometryCommit > > & uipc::core::SceneSnapshotCommit::geometries () noexcept const
```




<hr>



### function is\_valid 

```C++
inline bool uipc::core::SceneSnapshotCommit::is_valid () noexcept const
```




<hr>



### function object\_collection 

```C++
inline const ObjectCollectionSnapshot & uipc::core::SceneSnapshotCommit::object_collection () noexcept const
```




<hr>



### function rest\_geometries 

```C++
inline const unordered_map< IndexT, S< geometry::GeometryCommit > > & uipc::core::SceneSnapshotCommit::rest_geometries () noexcept const
```




<hr>## Friends Documentation





### friend Scene 

```C++
class uipc::core::SceneSnapshotCommit::Scene (
    internal::Scene
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/scene_snapshot.h`

