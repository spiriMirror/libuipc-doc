

# Class uipc::core::internal::Scene



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**internal**](namespaceuipc_1_1core_1_1internal.md) **>** [**Scene**](classuipc_1_1core_1_1internal_1_1_scene.md)








Inherits the following classes: std::enable_shared_from_this< Scene >


































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Scene**](#function-scene) (const Json & config) noexcept<br> |
|  auto & | [**animator**](#function-animator-12) () noexcept const<br> |
|  auto & | [**animator**](#function-animator-22) () noexcept<br> |
|  void | [**begin\_pending**](#function-begin_pending) () noexcept<br> |
|  auto & | [**config**](#function-config-12) () noexcept const<br> |
|  auto & | [**config**](#function-config-22) () noexcept<br> |
|  auto & | [**constitution\_tabular**](#function-constitution_tabular-12) () noexcept const<br> |
|  auto & | [**constitution\_tabular**](#function-constitution_tabular-22) () noexcept<br> |
|  auto & | [**contact\_tabular**](#function-contact_tabular-12) () noexcept const<br> |
|  auto & | [**contact\_tabular**](#function-contact_tabular-22) () noexcept<br> |
|  auto & | [**diff\_sim**](#function-diff_sim-12) () noexcept const<br> |
|  auto & | [**diff\_sim**](#function-diff_sim-22) () noexcept<br> |
|  Float | [**dt**](#function-dt) () noexcept const<br> |
|  auto & | [**geometries**](#function-geometries-12) () noexcept const<br> |
|  auto & | [**geometries**](#function-geometries-22) () noexcept<br> |
|  void | [**init**](#function-init) ([**internal::World**](classuipc_1_1core_1_1internal_1_1_world.md) & world) noexcept<br> |
|  bool | [**is\_pending**](#function-is_pending) () noexcept const<br> |
|  bool | [**is\_started**](#function-is_started) () noexcept const<br> |
|  auto & | [**objects**](#function-objects-12) () noexcept const<br> |
|  auto & | [**objects**](#function-objects-22) () noexcept<br> |
|  auto & | [**rest\_geometries**](#function-rest_geometries-12) () noexcept const<br> |
|  auto & | [**rest\_geometries**](#function-rest_geometries-22) () noexcept<br> |
|  auto & | [**sanity\_checker**](#function-sanity_checker-12) () noexcept const<br> |
|  auto & | [**sanity\_checker**](#function-sanity_checker-22) () noexcept<br> |
|  void | [**solve\_pending**](#function-solve_pending) () noexcept<br> |
|  auto & | [**subscene\_tabular**](#function-subscene_tabular-12) () noexcept const<br> |
|  auto & | [**subscene\_tabular**](#function-subscene_tabular-22) () noexcept<br> |
|  void | [**update\_from**](#function-update_from) (const [**SceneSnapshotCommit**](classuipc_1_1core_1_1_scene_snapshot_commit.md) & commit) <br> |
|  auto | [**world**](#function-world) () noexcept<br> |
|   | [**~Scene**](#function-scene) () <br> |




























## Public Functions Documentation




### function Scene 

```C++
uipc::core::internal::Scene::Scene (
    const Json & config
) noexcept
```




<hr>



### function animator [1/2]

```C++
inline auto & uipc::core::internal::Scene::animator () noexcept const
```




<hr>



### function animator [2/2]

```C++
inline auto & uipc::core::internal::Scene::animator () noexcept
```




<hr>



### function begin\_pending 

```C++
void uipc::core::internal::Scene::begin_pending () noexcept
```




<hr>



### function config [1/2]

```C++
inline auto & uipc::core::internal::Scene::config () noexcept const
```




<hr>



### function config [2/2]

```C++
inline auto & uipc::core::internal::Scene::config () noexcept
```




<hr>



### function constitution\_tabular [1/2]

```C++
inline auto & uipc::core::internal::Scene::constitution_tabular () noexcept const
```




<hr>



### function constitution\_tabular [2/2]

```C++
inline auto & uipc::core::internal::Scene::constitution_tabular () noexcept
```




<hr>



### function contact\_tabular [1/2]

```C++
inline auto & uipc::core::internal::Scene::contact_tabular () noexcept const
```




<hr>



### function contact\_tabular [2/2]

```C++
inline auto & uipc::core::internal::Scene::contact_tabular () noexcept
```




<hr>



### function diff\_sim [1/2]

```C++
inline auto & uipc::core::internal::Scene::diff_sim () noexcept const
```




<hr>



### function diff\_sim [2/2]

```C++
inline auto & uipc::core::internal::Scene::diff_sim () noexcept
```




<hr>



### function dt 

```C++
Float uipc::core::internal::Scene::dt () noexcept const
```




<hr>



### function geometries [1/2]

```C++
inline auto & uipc::core::internal::Scene::geometries () noexcept const
```




<hr>



### function geometries [2/2]

```C++
inline auto & uipc::core::internal::Scene::geometries () noexcept
```




<hr>



### function init 

```C++
void uipc::core::internal::Scene::init (
    internal::World & world
) noexcept
```




<hr>



### function is\_pending 

```C++
inline bool uipc::core::internal::Scene::is_pending () noexcept const
```




<hr>



### function is\_started 

```C++
inline bool uipc::core::internal::Scene::is_started () noexcept const
```




<hr>



### function objects [1/2]

```C++
inline auto & uipc::core::internal::Scene::objects () noexcept const
```




<hr>



### function objects [2/2]

```C++
inline auto & uipc::core::internal::Scene::objects () noexcept
```




<hr>



### function rest\_geometries [1/2]

```C++
inline auto & uipc::core::internal::Scene::rest_geometries () noexcept const
```




<hr>



### function rest\_geometries [2/2]

```C++
inline auto & uipc::core::internal::Scene::rest_geometries () noexcept
```




<hr>



### function sanity\_checker [1/2]

```C++
inline auto & uipc::core::internal::Scene::sanity_checker () noexcept const
```




<hr>



### function sanity\_checker [2/2]

```C++
inline auto & uipc::core::internal::Scene::sanity_checker () noexcept
```




<hr>



### function solve\_pending 

```C++
void uipc::core::internal::Scene::solve_pending () noexcept
```




<hr>



### function subscene\_tabular [1/2]

```C++
inline auto & uipc::core::internal::Scene::subscene_tabular () noexcept const
```




<hr>



### function subscene\_tabular [2/2]

```C++
inline auto & uipc::core::internal::Scene::subscene_tabular () noexcept
```




<hr>



### function update\_from 

```C++
void uipc::core::internal::Scene::update_from (
    const SceneSnapshotCommit & commit
) 
```




<hr>



### function world 

```C++
inline auto uipc::core::internal::Scene::world () noexcept
```




<hr>



### function ~Scene 

```C++
uipc::core::internal::Scene::~Scene () 
```




<hr>## Friends Documentation





### friend Scene 

```C++
class uipc::core::internal::Scene::Scene (
    core::Scene
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/internal/scene.h`

