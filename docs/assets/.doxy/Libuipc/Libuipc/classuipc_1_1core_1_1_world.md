

# Class uipc::core::World



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**World**](classuipc_1_1core_1_1_world.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**World**](#function-world) ([**Engine**](classuipc_1_1core_1_1_engine.md) & e) noexcept<br> |
|  void | [**advance**](#function-advance) () <br> |
|  void | [**backward**](#function-backward) () <br> |
|  bool | [**dump**](#function-dump) () <br> |
|  SizeT | [**frame**](#function-frame) () const<br> |
|  void | [**init**](#function-init) ([**Scene**](classuipc_1_1core_1_1_scene.md) & s) <br> |
|  bool | [**is\_valid**](#function-is_valid) () const<br> |
|  bool | [**recover**](#function-recover) (SizeT aim\_frame=~0ull) <br> |
|  void | [**retrieve**](#function-retrieve) () <br> |
|  void | [**sync**](#function-sync) () <br> |




























## Public Functions Documentation




### function World 

```C++
uipc::core::World::World (
    Engine & e
) noexcept
```




<hr>



### function advance 

```C++
void uipc::core::World::advance () 
```




<hr>



### function backward 

```C++
void uipc::core::World::backward () 
```




<hr>



### function dump 

```C++
bool uipc::core::World::dump () 
```




<hr>



### function frame 

```C++
SizeT uipc::core::World::frame () const
```




<hr>



### function init 

```C++
void uipc::core::World::init (
    Scene & s
) 
```




<hr>



### function is\_valid 

```C++
bool uipc::core::World::is_valid () const
```




<hr>



### function recover 

```C++
bool uipc::core::World::recover (
    SizeT aim_frame=~0ull
) 
```




<hr>



### function retrieve 

```C++
void uipc::core::World::retrieve () 
```




<hr>



### function sync 

```C++
void uipc::core::World::sync () 
```




<hr>## Friends Documentation





### friend WorldVisitor 

```C++
class uipc::core::World::WorldVisitor (
    backend::WorldVisitor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/world.h`

