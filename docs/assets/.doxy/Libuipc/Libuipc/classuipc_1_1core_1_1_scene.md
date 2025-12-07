

# Class uipc::core::Scene



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**Scene**](classuipc_1_1core_1_1_scene.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**CGeometries**](classuipc_1_1core_1_1_scene_1_1_c_geometries.md) <br> |
| class | [**CObjects**](classuipc_1_1core_1_1_scene_1_1_c_objects.md) <br> |
| class | [**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md) &lt;IsConst&gt;<br> |
| class | [**Geometries**](classuipc_1_1core_1_1_scene_1_1_geometries.md) <br> |
| class | [**Objects**](classuipc_1_1core_1_1_scene_1_1_objects.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md)&lt; true &gt; | [**CConfigAttributes**](#typedef-cconfigattributes)  <br> |
| typedef [**ConfigAttributesT**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md)&lt; false &gt; | [**ConfigAttributes**](#typedef-configattributes)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Scene**](#function-scene-14) (const Json & config=default\_config()) <br> |
|   | [**Scene**](#function-scene-24) (S&lt; [**internal::Scene**](classuipc_1_1core_1_1internal_1_1_scene.md) &gt; scene) noexcept<br> |
|   | [**Scene**](#function-scene-34) (const [**Scene**](classuipc_1_1core_1_1_scene.md) &) = delete<br> |
|   | [**Scene**](#function-scene-44) ([**Scene**](classuipc_1_1core_1_1_scene.md) &&) = default<br> |
|  [**Animator**](classuipc_1_1core_1_1_animator.md) & | [**animator**](#function-animator-12) () <br> |
|  const [**Animator**](classuipc_1_1core_1_1_animator.md) & | [**animator**](#function-animator-22) () const<br> |
|  [**ConfigAttributes**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md) | [**config**](#function-config-12) () noexcept<br> |
|  [**CConfigAttributes**](classuipc_1_1core_1_1_scene_1_1_config_attributes_t.md) | [**config**](#function-config-22) () noexcept const<br> |
|  [**ConstitutionTabular**](classuipc_1_1core_1_1_constitution_tabular.md) & | [**constitution\_tabular**](#function-constitution_tabular-12) () noexcept<br> |
|  const [**ConstitutionTabular**](classuipc_1_1core_1_1_constitution_tabular.md) & | [**constitution\_tabular**](#function-constitution_tabular-22) () noexcept const<br> |
|  [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) & | [**contact\_tabular**](#function-contact_tabular-12) () noexcept<br> |
|  const [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) & | [**contact\_tabular**](#function-contact_tabular-22) () noexcept const<br> |
|  [**DiffSim**](classuipc_1_1core_1_1_diff_sim.md) & | [**diff\_sim**](#function-diff_sim-12) () <br> |
|  const [**DiffSim**](classuipc_1_1core_1_1_diff_sim.md) & | [**diff\_sim**](#function-diff_sim-22) () const<br> |
|  [**Geometries**](classuipc_1_1core_1_1_scene_1_1_geometries.md) | [**geometries**](#function-geometries-12) () noexcept<br> |
|  [**CGeometries**](classuipc_1_1core_1_1_scene_1_1_c_geometries.md) | [**geometries**](#function-geometries-22) () noexcept const<br> |
|  [**Objects**](classuipc_1_1core_1_1_scene_1_1_objects.md) | [**objects**](#function-objects-12) () noexcept<br> |
|  [**CObjects**](classuipc_1_1core_1_1_scene_1_1_c_objects.md) | [**objects**](#function-objects-22) () noexcept const<br> |
|  [**SubsceneTabular**](classuipc_1_1core_1_1_subscene_tabular.md) & | [**subscene\_tabular**](#function-subscene_tabular-12) () noexcept<br> |
|  const [**SubsceneTabular**](classuipc_1_1core_1_1_subscene_tabular.md) & | [**subscene\_tabular**](#function-subscene_tabular-22) () noexcept const<br> |
|  void | [**update\_from**](#function-update_from) (const [**SceneSnapshotCommit**](classuipc_1_1core_1_1_scene_snapshot_commit.md) & snapshot) <br> |
|   | [**~Scene**](#function-scene) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Json | [**default\_config**](#function-default_config) () noexcept<br> |


























## Public Types Documentation




### typedef CConfigAttributes 

```C++
using uipc::core::Scene::CConfigAttributes =  ConfigAttributesT<true>;
```




<hr>



### typedef ConfigAttributes 

```C++
using uipc::core::Scene::ConfigAttributes =  ConfigAttributesT<false>;
```




<hr>
## Public Functions Documentation




### function Scene [1/4]

```C++
explicit uipc::core::Scene::Scene (
    const Json & config=default_config()
) 
```




<hr>



### function Scene [2/4]

```C++
explicit uipc::core::Scene::Scene (
    S< internal::Scene > scene
) noexcept
```




<hr>



### function Scene [3/4]

```C++
uipc::core::Scene::Scene (
    const Scene &
) = delete
```




<hr>



### function Scene [4/4]

```C++
uipc::core::Scene::Scene (
    Scene &&
) = default
```




<hr>



### function animator [1/2]

```C++
Animator & uipc::core::Scene::animator () 
```




<hr>



### function animator [2/2]

```C++
const Animator & uipc::core::Scene::animator () const
```




<hr>



### function config [1/2]

```C++
ConfigAttributes uipc::core::Scene::config () noexcept
```




<hr>



### function config [2/2]

```C++
CConfigAttributes uipc::core::Scene::config () noexcept const
```




<hr>



### function constitution\_tabular [1/2]

```C++
ConstitutionTabular & uipc::core::Scene::constitution_tabular () noexcept
```




<hr>



### function constitution\_tabular [2/2]

```C++
const ConstitutionTabular & uipc::core::Scene::constitution_tabular () noexcept const
```




<hr>



### function contact\_tabular [1/2]

```C++
ContactTabular & uipc::core::Scene::contact_tabular () noexcept
```




<hr>



### function contact\_tabular [2/2]

```C++
const ContactTabular & uipc::core::Scene::contact_tabular () noexcept const
```




<hr>



### function diff\_sim [1/2]

```C++
DiffSim & uipc::core::Scene::diff_sim () 
```




<hr>



### function diff\_sim [2/2]

```C++
const DiffSim & uipc::core::Scene::diff_sim () const
```




<hr>



### function geometries [1/2]

```C++
Geometries uipc::core::Scene::geometries () noexcept
```




<hr>



### function geometries [2/2]

```C++
CGeometries uipc::core::Scene::geometries () noexcept const
```




<hr>



### function objects [1/2]

```C++
Objects uipc::core::Scene::objects () noexcept
```




<hr>



### function objects [2/2]

```C++
CObjects uipc::core::Scene::objects () noexcept const
```




<hr>



### function subscene\_tabular [1/2]

```C++
SubsceneTabular & uipc::core::Scene::subscene_tabular () noexcept
```




<hr>



### function subscene\_tabular [2/2]

```C++
const SubsceneTabular & uipc::core::Scene::subscene_tabular () noexcept const
```




<hr>



### function update\_from 

```C++
void uipc::core::Scene::update_from (
    const SceneSnapshotCommit & snapshot
) 
```




<hr>



### function ~Scene 

```C++
uipc::core::Scene::~Scene () 
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::core::Scene::default_config () noexcept
```




<hr>## Friends Documentation





### friend SceneVisitor 

```C++
class uipc::core::Scene::SceneVisitor (
    backend::SceneVisitor
) 
```




<hr>



### friend formatter&lt; Scene &gt; 

```C++
struct uipc::core::Scene::formatter< Scene > (
    fmt::formatter< Scene >
) 
```




<hr>



### friend SanityChecker 

```C++
class uipc::core::Scene::SanityChecker (
    sanity_check::SanityChecker
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/scene.h`

