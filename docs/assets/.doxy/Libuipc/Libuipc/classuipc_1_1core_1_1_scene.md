

# Class uipc::core::Scene



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**Scene**](classuipc_1_1core_1_1_scene.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**CGeometries**](classuipc_1_1core_1_1_scene_1_1_c_geometries.md) <br> |
| class | [**CObjects**](classuipc_1_1core_1_1_scene_1_1_c_objects.md) <br> |
| class | [**Geometries**](classuipc_1_1core_1_1_scene_1_1_geometries.md) <br> |
| class | [**Objects**](classuipc_1_1core_1_1_scene_1_1_objects.md) <br> |






















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Scene**](#function-scene) (const Json & config=default\_config()) <br> |
|  [**Animator**](classuipc_1_1core_1_1_animator.md) & | [**animator**](#function-animator-12) () <br> |
|  const [**Animator**](classuipc_1_1core_1_1_animator.md) & | [**animator**](#function-animator-22) () const<br> |
|  const Json & | [**config**](#function-config) () noexcept const<br> |
|  [**ConstitutionTabular**](classuipc_1_1core_1_1_constitution_tabular.md) & | [**constitution\_tabular**](#function-constitution_tabular-12) () noexcept<br> |
|  const [**ConstitutionTabular**](classuipc_1_1core_1_1_constitution_tabular.md) & | [**constitution\_tabular**](#function-constitution_tabular-22) () noexcept const<br> |
|  [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) & | [**contact\_tabular**](#function-contact_tabular-12) () noexcept<br> |
|  const [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) & | [**contact\_tabular**](#function-contact_tabular-22) () noexcept const<br> |
|  [**DiffSim**](classuipc_1_1core_1_1_diff_sim.md) & | [**diff\_sim**](#function-diff_sim-12) () <br> |
|  const [**DiffSim**](classuipc_1_1core_1_1_diff_sim.md) & | [**diff\_sim**](#function-diff_sim-22) () const<br> |
|  [**Geometries**](classuipc_1_1core_1_1_scene_1_1_geometries.md) | [**geometries**](#function-geometries-12) () noexcept<br> |
|  [**CGeometries**](classuipc_1_1core_1_1_scene_1_1_c_geometries.md) | [**geometries**](#function-geometries-22) () noexcept const<br> |
|  const Json & | [**info**](#function-info) () noexcept const<br> |
|  [**Objects**](classuipc_1_1core_1_1_scene_1_1_objects.md) | [**objects**](#function-objects-12) () noexcept<br> |
|  [**CObjects**](classuipc_1_1core_1_1_scene_1_1_c_objects.md) | [**objects**](#function-objects-22) () noexcept const<br> |
|  [**SanityChecker**](classuipc_1_1core_1_1_sanity_checker.md) & | [**sanity\_checker**](#function-sanity_checker-12) () <br> |
|  const [**SanityChecker**](classuipc_1_1core_1_1_sanity_checker.md) & | [**sanity\_checker**](#function-sanity_checker-22) () const<br> |
|   | [**~Scene**](#function-scene) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Json | [**default\_config**](#function-default_config) () noexcept<br> |


























## Public Functions Documentation




### function Scene 

```C++
explicit uipc::core::Scene::Scene (
    const Json & config=default_config()
) 
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



### function config 

```C++
const Json & uipc::core::Scene::config () noexcept const
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



### function info 

```C++
const Json & uipc::core::Scene::info () noexcept const
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



### function sanity\_checker [1/2]

```C++
SanityChecker & uipc::core::Scene::sanity_checker () 
```




<hr>



### function sanity\_checker [2/2]

```C++
const SanityChecker & uipc::core::Scene::sanity_checker () const
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

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/scene.h`

