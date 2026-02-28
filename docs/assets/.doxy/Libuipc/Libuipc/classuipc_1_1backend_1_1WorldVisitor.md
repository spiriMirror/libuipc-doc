

# Class uipc::backend::WorldVisitor



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**backend**](namespaceuipc_1_1backend.md) **>** [**WorldVisitor**](classuipc_1_1backend_1_1WorldVisitor.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**WorldVisitor**](#function-worldvisitor-14) ([**core::World**](classuipc_1_1core_1_1World.md) & w) noexcept<br> |
|   | [**WorldVisitor**](#function-worldvisitor-24) ([**core::internal::World**](classuipc_1_1core_1_1internal_1_1World.md) & w) noexcept<br> |
|   | [**WorldVisitor**](#function-worldvisitor-34) (const [**WorldVisitor**](classuipc_1_1backend_1_1WorldVisitor.md) &) = delete<br> |
|   | [**WorldVisitor**](#function-worldvisitor-44) ([**WorldVisitor**](classuipc_1_1backend_1_1WorldVisitor.md) &&) = default<br> |
|  [**AnimatorVisitor**](classuipc_1_1backend_1_1AnimatorVisitor.md) | [**animator**](#function-animator) () noexcept<br> |
|  [**core::Engine**](classuipc_1_1core_1_1Engine.md) | [**engine**](#function-engine) () noexcept const<br> |
|  [**core::World**](classuipc_1_1core_1_1World.md) | [**get**](#function-get) () noexcept const<br> |
|  [**WorldVisitor**](classuipc_1_1backend_1_1WorldVisitor.md) & | [**operator=**](#function-operator) (const [**WorldVisitor**](classuipc_1_1backend_1_1WorldVisitor.md) &) = delete<br> |
|  [**WorldVisitor**](classuipc_1_1backend_1_1WorldVisitor.md) & | [**operator=**](#function-operator_1) ([**WorldVisitor**](classuipc_1_1backend_1_1WorldVisitor.md) &&) = delete<br> |
|  [**SceneVisitor**](classuipc_1_1backend_1_1SceneVisitor.md) | [**scene**](#function-scene) () noexcept<br> |




























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



### function engine 

```C++
core::Engine uipc::backend::WorldVisitor::engine () noexcept const
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
) = delete
```




<hr>



### function scene 

```C++
SceneVisitor uipc::backend::WorldVisitor::scene () noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/backend/visitors/world_visitor.h`

