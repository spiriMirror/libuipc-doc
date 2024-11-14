

# Namespace uipc::core



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**detail**](namespaceuipc_1_1core_1_1detail.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**Animation**](classuipc_1_1core_1_1_animation.md) <br> |
| class | [**Animator**](classuipc_1_1core_1_1_animator.md) <br> |
| class | [**ConstitutionTabular**](classuipc_1_1core_1_1_constitution_tabular.md) <br> |
| class | [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) <br> |
| class | [**ContactModel**](classuipc_1_1core_1_1_contact_model.md) <br> |
| class | [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) <br> |
| class | [**DiffSim**](classuipc_1_1core_1_1_diff_sim.md) <br> |
| class | [**Engine**](classuipc_1_1core_1_1_engine.md) <br> |
| class | [**EngineException**](classuipc_1_1core_1_1_engine_exception.md) <br> |
| class | [**EngineStatus**](classuipc_1_1core_1_1_engine_status.md) <br> |
| class | [**EngineStatusCollection**](classuipc_1_1core_1_1_engine_status_collection.md) <br> |
| class | [**IEngine**](classuipc_1_1core_1_1_i_engine.md) <br> |
| class | [**IObject**](classuipc_1_1core_1_1_i_object.md) <br> |
| class | [**IObjectCollection**](classuipc_1_1core_1_1_i_object_collection.md) <br> |
| class | [**ISanityChecker**](classuipc_1_1core_1_1_i_sanity_checker.md) <br> |
| class | [**Object**](classuipc_1_1core_1_1_object.md) <br> |
| class | [**ObjectCollection**](classuipc_1_1core_1_1_object_collection.md) <br> |
| class | [**ObjectGeometrySlots**](classuipc_1_1core_1_1_object_geometry_slots.md) &lt;GeometryT&gt;<br> |
| class | [**ObjectGeometrySlots&lt; const geometry::Geometry &gt;**](classuipc_1_1core_1_1_object_geometry_slots_3_01const_01geometry_1_1_geometry_01_4.md) &lt;&gt;<br> |
| class | [**ObjectGeometrySlots&lt; geometry::Geometry &gt;**](classuipc_1_1core_1_1_object_geometry_slots_3_01geometry_1_1_geometry_01_4.md) &lt;&gt;<br> |
| class | [**SanityChecker**](classuipc_1_1core_1_1_sanity_checker.md) <br> |
| class | [**SanityCheckerAutoRegister**](classuipc_1_1core_1_1_sanity_checker_auto_register.md) <br> |
| class | [**SanityCheckerCollection**](classuipc_1_1core_1_1_sanity_checker_collection.md) <br> |
| class | [**Scene**](classuipc_1_1core_1_1_scene.md) <br> |
| class | [**SceneIO**](classuipc_1_1core_1_1_scene_i_o.md) <br> |
| class | [**SceneIOError**](classuipc_1_1core_1_1_scene_i_o_error.md) <br> |
| class | [**World**](classuipc_1_1core_1_1_world.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| enum int | [**SanityCheckResult**](#enum-sanitycheckresult)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**from\_json**](#function-from_json) (const Json & j, [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & element) <br> |
|  void | [**from\_json**](#function-from_json) (const Json & json, [**ContactModel**](classuipc_1_1core_1_1_contact_model.md) & model) <br> |
|  void | [**to\_json**](#function-to_json) (Json & j, const [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & element) <br> |
|  void | [**to\_json**](#function-to_json) (Json & json, const [**ContactModel**](classuipc_1_1core_1_1_contact_model.md) & model) <br> |
|  void | [**to\_json**](#function-to_json) (Json & j, const [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) & ct) <br> |




























## Public Types Documentation




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

------------------------------
The documentation for this class was generated from the following file `include/uipc/backend/visitors/animator_visitor.h`

