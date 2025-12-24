

# Class uipc::core::SceneFactory



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SceneFactory**](classuipc_1_1core_1_1SceneFactory.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SceneFactory**](#function-scenefactory) () <br> |
|  [**SceneSnapshotCommit**](classuipc_1_1core_1_1SceneSnapshotCommit.md) | [**commit\_from\_json**](#function-commit_from_json) (const Json & json) <br> |
|  Json | [**commit\_to\_json**](#function-commit_to_json) (const [**SceneSnapshotCommit**](classuipc_1_1core_1_1SceneSnapshotCommit.md) & scene) <br> |
|  [**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md) | [**from\_json**](#function-from_json) (const Json & j) <br> |
|  [**Scene**](classuipc_1_1core_1_1Scene.md) | [**from\_snapshot**](#function-from_snapshot) (const [**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md) & snapshot) <br> |
|  Json | [**to\_json**](#function-to_json) (const [**SceneSnapshot**](classuipc_1_1core_1_1SceneSnapshot.md) & scene) <br> |
|   | [**~SceneFactory**](#function-scenefactory) () <br> |




























## Public Functions Documentation




### function SceneFactory 

```C++
uipc::core::SceneFactory::SceneFactory () 
```




<hr>



### function commit\_from\_json 

```C++
SceneSnapshotCommit uipc::core::SceneFactory::commit_from_json (
    const Json & json
) 
```




<hr>



### function commit\_to\_json 

```C++
Json uipc::core::SceneFactory::commit_to_json (
    const SceneSnapshotCommit & scene
) 
```




<hr>



### function from\_json 

```C++
SceneSnapshot uipc::core::SceneFactory::from_json (
    const Json & j
) 
```




<hr>



### function from\_snapshot 

```C++
Scene uipc::core::SceneFactory::from_snapshot (
    const SceneSnapshot & snapshot
) 
```




<hr>



### function to\_json 

```C++
Json uipc::core::SceneFactory::to_json (
    const SceneSnapshot & scene
) 
```




<hr>



### function ~SceneFactory 

```C++
uipc::core::SceneFactory::~SceneFactory () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/scene_factory.h`

