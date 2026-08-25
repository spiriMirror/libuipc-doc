

# Class uipc::core::SceneSnapshotCommit



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SceneSnapshotCommit**](classuipc_1_1core_1_1SceneSnapshotCommit.md)



[More...](#detailed-description)

* `#include <scene_snapshot.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SceneSnapshotCommit**](#function-scenesnapshotcommit-12) () = default<br> |
|   | [**SceneSnapshotCommit**](#function-scenesnapshotcommit-22) (const [**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md) & dst, const [**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md) & src) <br> |
|  const [**geometry::AttributeCollectionCommit**](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) & | [**config**](#function-config) () noexcept const<br> |
|  bool | [**contact\_default\_model\_is\_user\_set**](#function-contact_default_model_is_user_set) () noexcept const<br> |
|  const vector&lt; [**ContactElement**](classuipc_1_1core_1_1ContactElement.md) &gt; & | [**contact\_elements**](#function-contact_elements) () noexcept const<br> |
|  const [**geometry::AttributeCollectionCommit**](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) & | [**contact\_models**](#function-contact_models) () noexcept const<br> |
|  const unordered\_map&lt; IndexT, S&lt; [**geometry::GeometryCommit**](classuipc_1_1geometry_1_1GeometryCommit.md) &gt; &gt; & | [**geometries**](#function-geometries) () noexcept const<br> |
|  IndexT | [**geometry\_next\_id**](#function-geometry_next_id) () noexcept const<br> |
|  bool | [**is\_valid**](#function-is_valid) () noexcept const<br> |
|  const [**ObjectCollectionSnapshot**](classuipc_1_1core_1_1ObjectCollectionSnapshot.md) & | [**object\_collection**](#function-object_collection) () noexcept const<br> |
|  span&lt; const IndexT &gt; | [**removed\_geometry\_ids**](#function-removed_geometry_ids) () noexcept const<br> |
|  span&lt; const IndexT &gt; | [**removed\_rest\_geometry\_ids**](#function-removed_rest_geometry_ids) () noexcept const<br> |
|  const unordered\_map&lt; IndexT, S&lt; [**geometry::GeometryCommit**](classuipc_1_1geometry_1_1GeometryCommit.md) &gt; &gt; & | [**rest\_geometries**](#function-rest_geometries) () noexcept const<br> |
|  IndexT | [**rest\_geometry\_next\_id**](#function-rest_geometry_next_id) () noexcept const<br> |
|  const vector&lt; [**SubsceneElement**](classuipc_1_1core_1_1SubsceneElement.md) &gt; & | [**subscene\_elements**](#function-subscene_elements) () noexcept const<br> |
|  const [**geometry::AttributeCollectionCommit**](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) & | [**subscene\_models**](#function-subscene_models) () noexcept const<br> |




























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



### function contact\_default\_model\_is\_user\_set 

```C++
inline bool uipc::core::SceneSnapshotCommit::contact_default_model_is_user_set () noexcept const
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



### function geometry\_next\_id 

```C++
inline IndexT uipc::core::SceneSnapshotCommit::geometry_next_id () noexcept const
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



### function removed\_geometry\_ids 

```C++
inline span< const IndexT > uipc::core::SceneSnapshotCommit::removed_geometry_ids () noexcept const
```




<hr>



### function removed\_rest\_geometry\_ids 

```C++
inline span< const IndexT > uipc::core::SceneSnapshotCommit::removed_rest_geometry_ids () noexcept const
```




<hr>



### function rest\_geometries 

```C++
inline const unordered_map< IndexT, S< geometry::GeometryCommit > > & uipc::core::SceneSnapshotCommit::rest_geometries () noexcept const
```




<hr>



### function rest\_geometry\_next\_id 

```C++
inline IndexT uipc::core::SceneSnapshotCommit::rest_geometry_next_id () noexcept const
```




<hr>



### function subscene\_elements 

```C++
inline const vector< SubsceneElement > & uipc::core::SceneSnapshotCommit::subscene_elements () noexcept const
```




<hr>



### function subscene\_models 

```C++
inline const geometry::AttributeCollectionCommit & uipc::core::SceneSnapshotCommit::subscene_models () noexcept const
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

