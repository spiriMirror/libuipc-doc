

# Namespace uipc::core



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**internal**](namespaceuipc_1_1core_1_1internal.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**Animation**](classuipc_1_1core_1_1_animation.md) <br> |
| class | [**Animator**](classuipc_1_1core_1_1_animator.md) <br> |
| class | [**ConstitutionTabular**](classuipc_1_1core_1_1_constitution_tabular.md) <br> |
| class | [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) <br> |
| class | [**ContactModel**](classuipc_1_1core_1_1_contact_model.md) <br> |
| class | [**ContactModelCollectionT**](classuipc_1_1core_1_1_contact_model_collection_t.md) &lt;IsConst&gt;<br> |
| class | [**ContactSystemFeature**](classuipc_1_1core_1_1_contact_system_feature.md) <br> |
| class | [**ContactSystemFeatureOverrider**](classuipc_1_1core_1_1_contact_system_feature_overrider.md) <br> |
| class | [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) <br> |
| class | [**DiffSim**](classuipc_1_1core_1_1_diff_sim.md) <br> |
| class | [**Engine**](classuipc_1_1core_1_1_engine.md) <br> |
| class | [**EngineException**](classuipc_1_1core_1_1_engine_exception.md) <br> |
| class | [**EngineStatus**](classuipc_1_1core_1_1_engine_status.md) <br> |
| class | [**EngineStatusCollection**](classuipc_1_1core_1_1_engine_status_collection.md) <br> |
| class | [**Feature**](classuipc_1_1core_1_1_feature.md) <br> |
| class | [**FeatureCollection**](classuipc_1_1core_1_1_feature_collection.md) <br> |
| class | [**IEngine**](classuipc_1_1core_1_1_i_engine.md) <br> |
| class | [**IFeature**](classuipc_1_1core_1_1_i_feature.md) <br> |
| class | [**IObject**](classuipc_1_1core_1_1_i_object.md) <br> |
| class | [**IObjectCollection**](classuipc_1_1core_1_1_i_object_collection.md) <br> |
| class | [**ISanityChecker**](classuipc_1_1core_1_1_i_sanity_checker.md) <br> |
| class | [**ISanityCheckerCollection**](classuipc_1_1core_1_1_i_sanity_checker_collection.md) <br> |
| class | [**Object**](classuipc_1_1core_1_1_object.md) <br> |
| class | [**ObjectCollection**](classuipc_1_1core_1_1_object_collection.md) <br> |
| class | [**ObjectCollectionSnapshot**](classuipc_1_1core_1_1_object_collection_snapshot.md) <br> |
| class | [**ObjectGeometrySlots**](classuipc_1_1core_1_1_object_geometry_slots.md) &lt;GeometryT&gt;<br> |
| class | [**ObjectGeometrySlots&lt; const geometry::Geometry &gt;**](classuipc_1_1core_1_1_object_geometry_slots_3_01const_01geometry_1_1_geometry_01_4.md) &lt;&gt;<br> |
| class | [**ObjectGeometrySlots&lt; geometry::Geometry &gt;**](classuipc_1_1core_1_1_object_geometry_slots_3_01geometry_1_1_geometry_01_4.md) &lt;&gt;<br> |
| class | [**ObjectSnapshot**](classuipc_1_1core_1_1_object_snapshot.md) <br> |
| class | [**SanityCheckMessage**](classuipc_1_1core_1_1_sanity_check_message.md) <br> |
| class | [**SanityCheckMessageCollection**](classuipc_1_1core_1_1_sanity_check_message_collection.md) <br> |
| class | [**SanityChecker**](classuipc_1_1core_1_1_sanity_checker.md) <br> |
| class | [**SanityCheckerCollectionCreateInfo**](classuipc_1_1core_1_1_sanity_checker_collection_create_info.md) <br> |
| class | [**Scene**](classuipc_1_1core_1_1_scene.md) <br> |
| class | [**SceneFactory**](classuipc_1_1core_1_1_scene_factory.md) <br> |
| class | [**SceneIO**](classuipc_1_1core_1_1_scene_i_o.md) <br> |
| class | [**SceneIOError**](classuipc_1_1core_1_1_scene_i_o_error.md) <br> |
| class | [**SceneSnapshot**](classuipc_1_1core_1_1_scene_snapshot.md) <br> |
| class | [**SceneSnapshotCommit**](classuipc_1_1core_1_1_scene_snapshot_commit.md) <br> |
| class | [**World**](classuipc_1_1core_1_1_world.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**ContactModelCollectionT**](classuipc_1_1core_1_1_contact_model_collection_t.md)&lt; true &gt; | [**CContactModelCollection**](#typedef-ccontactmodelcollection)  <br> |
| typedef [**ContactModelCollectionT**](classuipc_1_1core_1_1_contact_model_collection_t.md)&lt; false &gt; | [**ContactModelCollection**](#typedef-contactmodelcollection)  <br> |
| enum int | [**SanityCheckResult**](#enum-sanitycheckresult)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**from\_json**](#function-from_json) (const Json & j, [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & element) <br> |
|  void | [**from\_json**](#function-from_json) (const Json & json, [**ContactModel**](classuipc_1_1core_1_1_contact_model.md) & model) <br> |
|  void | [**from\_json**](#function-from_json) (const Json & j, [**Object**](classuipc_1_1core_1_1_object.md) & object) noexcept<br> |
|  void UIPC\_CORE\_API | [**from\_json**](#function-from_json) (const Json & j, [**ObjectCollectionSnapshot**](classuipc_1_1core_1_1_object_collection_snapshot.md) & obj) <br> |
|  UIPC\_CORE\_API void | [**from\_json**](#function-from_json) (const Json & j, [**ObjectSnapshot**](classuipc_1_1core_1_1_object_snapshot.md) & snapshot) <br> |
|  [**SceneSnapshotCommit**](classuipc_1_1core_1_1_scene_snapshot_commit.md) UIPC\_CORE\_API | [**operator-**](#function-operator) (const [**SceneSnapshot**](classuipc_1_1core_1_1_scene_snapshot.md) & dst, const [**SceneSnapshot**](classuipc_1_1core_1_1_scene_snapshot.md) & src) <br> |
|  void | [**to\_json**](#function-to_json) (Json & j, const [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & element) <br> |
|  void | [**to\_json**](#function-to_json) (Json & json, const [**ContactModel**](classuipc_1_1core_1_1_contact_model.md) & model) <br> |
|  void | [**to\_json**](#function-to_json) (Json & j, const [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) & ct) <br> |
|  void | [**to\_json**](#function-to_json) (Json & j, const [**Object**](classuipc_1_1core_1_1_object.md) & object) noexcept<br> |
|  void UIPC\_CORE\_API | [**to\_json**](#function-to_json) (Json & j, const [**ObjectCollectionSnapshot**](classuipc_1_1core_1_1_object_collection_snapshot.md) & obj) <br> |
|  UIPC\_CORE\_API void | [**to\_json**](#function-to_json) (Json & j, const [**ObjectSnapshot**](classuipc_1_1core_1_1_object_snapshot.md) & snapshot) <br> |




























## Public Types Documentation




### typedef CContactModelCollection 

```C++
using uipc::core::CContactModelCollection = typedef ContactModelCollectionT<true>;
```




<hr>



### typedef ContactModelCollection 

```C++
using uipc::core::ContactModelCollection = typedef ContactModelCollectionT<false>;
```




<hr>



### enum SanityCheckResult 

```C++
enum uipc::core::SanityCheckResult {
    Success = 0,
    Warning = 1,
    Error = 2
};
```




<hr>
## Public Functions Documentation




### function from\_json 

```C++
void uipc::core::from_json (
    const Json & j,
    ContactElement & element
) 
```




<hr>



### function from\_json 

```C++
void uipc::core::from_json (
    const Json & json,
    ContactModel & model
) 
```




<hr>



### function from\_json 

```C++
void uipc::core::from_json (
    const Json & j,
    Object & object
) noexcept
```




<hr>



### function from\_json 

```C++
void UIPC_CORE_API uipc::core::from_json (
    const Json & j,
    ObjectCollectionSnapshot & obj
) 
```




<hr>



### function from\_json 

```C++
UIPC_CORE_API void uipc::core::from_json (
    const Json & j,
    ObjectSnapshot & snapshot
) 
```




<hr>



### function operator- 

```C++
SceneSnapshotCommit UIPC_CORE_API uipc::core::operator- (
    const SceneSnapshot & dst,
    const SceneSnapshot & src
) 
```




<hr>



### function to\_json 

```C++
void uipc::core::to_json (
    Json & j,
    const ContactElement & element
) 
```




<hr>



### function to\_json 

```C++
void uipc::core::to_json (
    Json & json,
    const ContactModel & model
) 
```




<hr>



### function to\_json 

```C++
void uipc::core::to_json (
    Json & j,
    const ContactTabular & ct
) 
```




<hr>



### function to\_json 

```C++
void uipc::core::to_json (
    Json & j,
    const Object & object
) noexcept
```




<hr>



### function to\_json 

```C++
void UIPC_CORE_API uipc::core::to_json (
    Json & j,
    const ObjectCollectionSnapshot & obj
) 
```




<hr>



### function to\_json 

```C++
UIPC_CORE_API void uipc::core::to_json (
    Json & j,
    const ObjectSnapshot & snapshot
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/backend/visitors/animator_visitor.h`

