

# Class uipc::core::SceneSnapshot



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md)



[More...](#detailed-description)

* `#include <scene_snapshot.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SceneSnapshot**](#function-scenesnapshot-14) (const [**Scene**](classuipc_1_1core_1_1Scene.md) & scene) <br> |
|   | [**SceneSnapshot**](#function-scenesnapshot-24) (const [**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md) &) = default<br> |
|   | [**SceneSnapshot**](#function-scenesnapshot-34) ([**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md) &&) = default<br> |
|  [**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md) & | [**operator=**](#function-operator) (const [**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md) &) = default<br> |
|  [**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md) & | [**operator=**](#function-operator_1) ([**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md) &&) = default<br> |




























## Detailed Description


Create a scene snapshot from the given scene, which is a plain data copy of the scene (detached from the world). 


    
## Public Functions Documentation




### function SceneSnapshot [1/4]

```C++
uipc::core::SceneSnapshot::SceneSnapshot (
    const Scene & scene
) 
```




<hr>



### function SceneSnapshot [2/4]

```C++
uipc::core::SceneSnapshot::SceneSnapshot (
    const SceneSnapshot &
) = default
```




<hr>



### function SceneSnapshot [3/4]

```C++
uipc::core::SceneSnapshot::SceneSnapshot (
    SceneSnapshot &&
) = default
```




<hr>



### function operator= 

```C++
SceneSnapshot & uipc::core::SceneSnapshot::operator= (
    const SceneSnapshot &
) = default
```




<hr>



### function operator= 

```C++
SceneSnapshot & uipc::core::SceneSnapshot::operator= (
    SceneSnapshot &&
) = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/scene_snapshot.h`

