

# Class uipc::backend::SceneVisitor



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**backend**](namespaceuipc_1_1backend.md) **>** [**SceneVisitor**](classuipc_1_1backend_1_1_scene_visitor.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SceneVisitor**](#function-scenevisitor) ([**core::Scene**](classuipc_1_1core_1_1_scene.md) & scene) noexcept<br> |
|  void | [**begin\_pending**](#function-begin_pending) () noexcept<br> |
|  const [**core::ConstitutionTabular**](classuipc_1_1core_1_1_constitution_tabular.md) & | [**constitution\_tabular**](#function-constitution_tabular) () noexcept const<br> |
|  const [**core::ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) & | [**contact\_tabular**](#function-contact_tabular) () noexcept const<br> |
|  const [**DiffSimVisitor**](classuipc_1_1backend_1_1_diff_sim_visitor.md) & | [**diff\_sim**](#function-diff_sim-12) () noexcept const<br> |
|  [**DiffSimVisitor**](classuipc_1_1backend_1_1_diff_sim_visitor.md) & | [**diff\_sim**](#function-diff_sim-22) () noexcept<br> |
|  S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; | [**find\_geometry**](#function-find_geometry) (IndexT id) noexcept<br> |
|  S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; | [**find\_rest\_geometry**](#function-find_rest_geometry) (IndexT id) noexcept<br> |
|  span&lt; S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; &gt; | [**geometries**](#function-geometries) () noexcept const<br> |
|  const Json & | [**info**](#function-info) () noexcept const<br> |
|  span&lt; IndexT &gt; | [**pending\_destroy\_ids**](#function-pending_destroy_ids) () noexcept const<br> |
|  span&lt; S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; &gt; | [**pending\_geometries**](#function-pending_geometries) () noexcept const<br> |
|  span&lt; S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; &gt; | [**pending\_rest\_geometries**](#function-pending_rest_geometries) () noexcept const<br> |
|  span&lt; S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; &gt; | [**rest\_geometries**](#function-rest_geometries) () noexcept const<br> |
|  void | [**solve\_pending**](#function-solve_pending) () noexcept<br> |




























## Public Functions Documentation




### function SceneVisitor 

```C++
uipc::backend::SceneVisitor::SceneVisitor (
    core::Scene & scene
) noexcept
```




<hr>



### function begin\_pending 

```C++
void uipc::backend::SceneVisitor::begin_pending () noexcept
```




<hr>



### function constitution\_tabular 

```C++
const core::ConstitutionTabular & uipc::backend::SceneVisitor::constitution_tabular () noexcept const
```




<hr>



### function contact\_tabular 

```C++
const core::ContactTabular & uipc::backend::SceneVisitor::contact_tabular () noexcept const
```




<hr>



### function diff\_sim [1/2]

```C++
const DiffSimVisitor & uipc::backend::SceneVisitor::diff_sim () noexcept const
```




<hr>



### function diff\_sim [2/2]

```C++
DiffSimVisitor & uipc::backend::SceneVisitor::diff_sim () noexcept
```




<hr>



### function find\_geometry 

```C++
S< geometry::GeometrySlot > uipc::backend::SceneVisitor::find_geometry (
    IndexT id
) noexcept
```




<hr>



### function find\_rest\_geometry 

```C++
S< geometry::GeometrySlot > uipc::backend::SceneVisitor::find_rest_geometry (
    IndexT id
) noexcept
```




<hr>



### function geometries 

```C++
span< S< geometry::GeometrySlot > > uipc::backend::SceneVisitor::geometries () noexcept const
```




<hr>



### function info 

```C++
const Json & uipc::backend::SceneVisitor::info () noexcept const
```




<hr>



### function pending\_destroy\_ids 

```C++
span< IndexT > uipc::backend::SceneVisitor::pending_destroy_ids () noexcept const
```




<hr>



### function pending\_geometries 

```C++
span< S< geometry::GeometrySlot > > uipc::backend::SceneVisitor::pending_geometries () noexcept const
```




<hr>



### function pending\_rest\_geometries 

```C++
span< S< geometry::GeometrySlot > > uipc::backend::SceneVisitor::pending_rest_geometries () noexcept const
```




<hr>



### function rest\_geometries 

```C++
span< S< geometry::GeometrySlot > > uipc::backend::SceneVisitor::rest_geometries () noexcept const
```




<hr>



### function solve\_pending 

```C++
void uipc::backend::SceneVisitor::solve_pending () noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/backend/visitors/scene_visitor.h`

