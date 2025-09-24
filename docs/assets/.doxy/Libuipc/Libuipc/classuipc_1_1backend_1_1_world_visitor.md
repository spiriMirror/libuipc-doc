

# Class uipc::backend::WorldVisitor



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**backend**](namespaceuipc_1_1backend.md) **>** [**WorldVisitor**](classuipc_1_1backend_1_1_world_visitor.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**WorldVisitor**](#function-worldvisitor-14) ([**core::World**](classuipc_1_1core_1_1_world.md) & w) noexcept<br> |
|   | [**WorldVisitor**](#function-worldvisitor-24) ([**core::internal::World**](classuipc_1_1core_1_1internal_1_1_world.md) & w) noexcept<br> |
|   | [**WorldVisitor**](#function-worldvisitor-34) (const [**WorldVisitor**](classuipc_1_1backend_1_1_world_visitor.md) &) = delete<br> |
|   | [**WorldVisitor**](#function-worldvisitor-44) ([**WorldVisitor**](classuipc_1_1backend_1_1_world_visitor.md) &&) = default<br> |
|  [**AnimatorVisitor**](classuipc_1_1backend_1_1_animator_visitor.md) | [**animator**](#function-animator) () noexcept<br> |
|  [**core::World**](classuipc_1_1core_1_1_world.md) | [**get**](#function-get) () noexcept const<br> |
|  [**WorldVisitor**](classuipc_1_1backend_1_1_world_visitor.md) & | [**operator=**](#function-operator) (const [**WorldVisitor**](classuipc_1_1backend_1_1_world_visitor.md) &) = delete<br> |
|  [**WorldVisitor**](classuipc_1_1backend_1_1_world_visitor.md) & | [**operator=**](#function-operator_1) ([**WorldVisitor**](classuipc_1_1backend_1_1_world_visitor.md) &&) = default<br> |
|  [**SceneVisitor**](classuipc_1_1backend_1_1_scene_visitor.md) | [**scene**](#function-scene) () noexcept<br> |




























## Public Functions Documentation




### function WorldVisitor [1/4]

```C++
uipc::backend::WorldVisitor::WorldVisitor (
    core::World & w
) noexcept
```




<hr>



### function WorldVisitor [2/4]

```C++
uipc::backend::WorldVisitor::WorldVisitor (
    core::internal::World & w
) noexcept
```




<hr>



### function WorldVisitor [3/4]

```C++
uipc::backend::WorldVisitor::WorldVisitor (
    const WorldVisitor &
) = delete
```




<hr>



### function WorldVisitor [4/4]

```C++
uipc::backend::WorldVisitor::WorldVisitor (
    WorldVisitor &&
) = default
```




<hr>



### function animator 

```C++
AnimatorVisitor uipc::backend::WorldVisitor::animator () noexcept
```




<hr>



### function get 

```C++
core::World uipc::backend::WorldVisitor::get () noexcept const
```




<hr>



### function operator= 

```C++
WorldVisitor & uipc::backend::WorldVisitor::operator= (
    const WorldVisitor &
) = delete
```




<hr>



### function operator= 

```C++
WorldVisitor & uipc::backend::WorldVisitor::operator= (
    WorldVisitor &&
) = default
```




<hr>



### function scene 

```C++
SceneVisitor uipc::backend::WorldVisitor::scene () noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/backend/visitors/world_visitor.h`

