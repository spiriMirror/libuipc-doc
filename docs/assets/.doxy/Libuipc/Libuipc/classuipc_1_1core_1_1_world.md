

# Class uipc::core::World



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**World**](classuipc_1_1core_1_1_world.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**World**](#function-world-14) ([**Engine**](classuipc_1_1core_1_1_engine.md) & e) noexcept<br> |
|   | [**World**](#function-world-24) (const [**World**](classuipc_1_1core_1_1_world.md) &) = delete<br> |
|   | [**World**](#function-world-34) ([**World**](classuipc_1_1core_1_1_world.md) &&) = default<br> |
|   | [**World**](#function-world-44) (S&lt; [**internal::World**](classuipc_1_1core_1_1internal_1_1_world.md) &gt; w) noexcept<br> |
|  void | [**advance**](#function-advance) () <br> |
|  bool | [**dump**](#function-dump) () <br> |
|  const [**FeatureCollection**](classuipc_1_1core_1_1_feature_collection.md) & | [**features**](#function-features) () const<br> |
|  SizeT | [**frame**](#function-frame) () const<br> |
|  void | [**init**](#function-init) ([**Scene**](classuipc_1_1core_1_1_scene.md) & s) <br> |
|  bool | [**is\_valid**](#function-is_valid) () const<br> |
|  [**World**](classuipc_1_1core_1_1_world.md) & | [**operator=**](#function-operator) (const [**World**](classuipc_1_1core_1_1_world.md) &) = delete<br> |
|  [**World**](classuipc_1_1core_1_1_world.md) & | [**operator=**](#function-operator_1) ([**World**](classuipc_1_1core_1_1_world.md) &&) = default<br> |
|  bool | [**recover**](#function-recover) (SizeT aim\_frame=~0ull) <br> |
|  void | [**retrieve**](#function-retrieve) () <br> |
|  [**SanityChecker**](classuipc_1_1core_1_1_sanity_checker.md) & | [**sanity\_checker**](#function-sanity_checker-12) () <br> |
|  const [**SanityChecker**](classuipc_1_1core_1_1_sanity_checker.md) & | [**sanity\_checker**](#function-sanity_checker-22) () const<br> |
|  void | [**sync**](#function-sync) () <br> |
|   | [**~World**](#function-world) () <br> |




























## Public Functions Documentation




### function World [1/4]

```C++
uipc::core::World::World (
    Engine & e
) noexcept
```




<hr>



### function World [2/4]

```C++
uipc::core::World::World (
    const World &
) = delete
```




<hr>



### function World [3/4]

```C++
uipc::core::World::World (
    World &&
) = default
```




<hr>



### function World [4/4]

```C++
uipc::core::World::World (
    S< internal::World > w
) noexcept
```




<hr>



### function advance 

```C++
void uipc::core::World::advance () 
```




<hr>



### function dump 

```C++
bool uipc::core::World::dump () 
```




<hr>



### function features 

```C++
const FeatureCollection & uipc::core::World::features () const
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



### function operator= 

```C++
World & uipc::core::World::operator= (
    const World &
) = delete
```




<hr>



### function operator= 

```C++
World & uipc::core::World::operator= (
    World &&
) = default
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



### function sanity\_checker [1/2]

```C++
SanityChecker & uipc::core::World::sanity_checker () 
```




<hr>



### function sanity\_checker [2/2]

```C++
const SanityChecker & uipc::core::World::sanity_checker () const
```




<hr>



### function sync 

```C++
void uipc::core::World::sync () 
```




<hr>



### function ~World 

```C++
uipc::core::World::~World () 
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

