

# Class uipc::core::internal::World



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**internal**](namespaceuipc_1_1core_1_1internal.md) **>** [**World**](classuipc_1_1core_1_1internal_1_1World.md)








Inherits the following classes: std::enable_shared_from_this< World >


































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**World**](#function-world) ([**internal::Engine**](classuipc_1_1core_1_1internal_1_1Engine.md) & e) noexcept<br> |
|  void | [**advance**](#function-advance) () <br> |
|  bool | [**dump**](#function-dump) () <br> |
|  const [**FeatureCollection**](classuipc_1_1core_1_1FeatureCollection.md) & | [**features**](#function-features) () const<br> |
|  SizeT | [**frame**](#function-frame) () const<br> |
|  void | [**init**](#function-init) ([**internal::Scene**](classuipc_1_1core_1_1internal_1_1Scene.md) & s) <br> |
|  bool | [**is\_valid**](#function-is_valid) () const<br> |
|  bool | [**recover**](#function-recover) (SizeT aim\_frame=~0ull) <br> |
|  void | [**retrieve**](#function-retrieve) () <br> |
|  [**SanityChecker**](classuipc_1_1core_1_1SanityChecker.md) & | [**sanity\_checker**](#function-sanity_checker-12) () <br> |
|  const [**SanityChecker**](classuipc_1_1core_1_1SanityChecker.md) & | [**sanity\_checker**](#function-sanity_checker-22) () const<br> |
|  void | [**sync**](#function-sync) () <br> |




























## Public Functions Documentation




### function World 

```C++
uipc::core::internal::World::World (
    internal::Engine & e
) noexcept
```




<hr>



### function advance 

```C++
void uipc::core::internal::World::advance () 
```




<hr>



### function dump 

```C++
bool uipc::core::internal::World::dump () 
```




<hr>



### function features 

```C++
const FeatureCollection & uipc::core::internal::World::features () const
```




<hr>



### function frame 

```C++
SizeT uipc::core::internal::World::frame () const
```




<hr>



### function init 

```C++
void uipc::core::internal::World::init (
    internal::Scene & s
) 
```




<hr>



### function is\_valid 

```C++
bool uipc::core::internal::World::is_valid () const
```




<hr>



### function recover 

```C++
bool uipc::core::internal::World::recover (
    SizeT aim_frame=~0ull
) 
```




<hr>



### function retrieve 

```C++
void uipc::core::internal::World::retrieve () 
```




<hr>



### function sanity\_checker [1/2]

```C++
SanityChecker & uipc::core::internal::World::sanity_checker () 
```




<hr>



### function sanity\_checker [2/2]

```C++
const SanityChecker & uipc::core::internal::World::sanity_checker () const
```




<hr>



### function sync 

```C++
void uipc::core::internal::World::sync () 
```




<hr>## Friends Documentation





### friend WorldVisitor 

```C++
class uipc::core::internal::World::WorldVisitor (
    backend::WorldVisitor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/internal/world.h`

