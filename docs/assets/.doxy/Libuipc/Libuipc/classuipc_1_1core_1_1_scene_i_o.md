

# Class uipc::core::SceneIO



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SceneIO**](classuipc_1_1core_1_1_scene_i_o.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SceneIO**](#function-sceneio) ([**Scene**](classuipc_1_1core_1_1_scene.md) & scene) <br> |
|  void | [**commit**](#function-commit) (const [**SceneSnapshot**](classuipc_1_1core_1_1_scene_snapshot.md) & reference, std::string\_view filename) <br>_Commit the scene's update to a file._  |
|  Json | [**commit\_to\_json**](#function-commit_to_json) (const [**SceneSnapshot**](classuipc_1_1core_1_1_scene_snapshot.md) & reference) const<br>_Commit the scene's update to a json object._  |
|  void | [**save**](#function-save-12) (std::string\_view filename) const<br>_Save the scene to a file._  |
|  [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**simplicial\_surface**](#function-simplicial_surface) (IndexT dim=-1) const<br>_Get the surface of the scene in the form of a simplicial complex allow to specify the dimension of the surface._  |
|  Json | [**to\_json**](#function-to_json) () const<br>_Convert the scene to a json object._  |
|  void | [**update**](#function-update) (std::string\_view filename) <br>_Update the scene from a SnapshotCommit file._  |
|  void | [**update\_from\_json**](#function-update_from_json) (const Json & json) <br>_Update the scene from a scene commit json object._  |
|  void | [**write\_surface**](#function-write_surface) (std::string\_view filename) <br>_Write the surface of the scene to a file. Supported formats:_  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**Scene**](classuipc_1_1core_1_1_scene.md) | [**from\_json**](#function-from_json) (const Json & json) <br>_Convert a json object to a scene._  |
|  [**Scene**](classuipc_1_1core_1_1_scene.md) | [**load**](#function-load) (std::string\_view filename) <br>_Load a scene from a file._  |
|  void | [**save**](#function-save-22) (const [**Scene**](classuipc_1_1core_1_1_scene.md) & scene, std::string\_view filename) <br>_Save the scene to a file._  |


























## Public Functions Documentation




### function SceneIO 

```C++
uipc::core::SceneIO::SceneIO (
    Scene & scene
) 
```




<hr>



### function commit 

_Commit the scene's update to a file._ 
```C++
void uipc::core::SceneIO::commit (
    const SceneSnapshot & reference,
    std::string_view filename
) 
```



Supported formats:
* .json
* .bson






**Parameters:**


* `reference` 
* `filename` 




        

<hr>



### function commit\_to\_json 

_Commit the scene's update to a json object._ 
```C++
Json uipc::core::SceneIO::commit_to_json (
    const SceneSnapshot & reference
) const
```



Supported formats:
* .json
* .bson






**Parameters:**


* `reference` 
* `filename` 




        

<hr>



### function save [1/2]

_Save the scene to a file._ 
```C++
void uipc::core::SceneIO::save (
    std::string_view filename
) const
```



Supported formats:
* .json
* .bson






**Parameters:**


* `filename` 




        

<hr>



### function simplicial\_surface 

_Get the surface of the scene in the form of a simplicial complex allow to specify the dimension of the surface._ 
```C++
geometry::SimplicialComplex uipc::core::SceneIO::simplicial_surface (
    IndexT dim=-1
) const
```




* 0: point cloud
* 1: line mesh
* 2: triangle mesh
* -1: all dimensions 

**Parameters:**


  * `dim` 



**Returns:**









        

<hr>



### function to\_json 

_Convert the scene to a json object._ 
```C++
Json uipc::core::SceneIO::to_json () const
```





**Returns:**







        

<hr>



### function update 

_Update the scene from a SnapshotCommit file._ 
```C++
void uipc::core::SceneIO::update (
    std::string_view filename
) 
```



Supported formats:
* - .json
* .bson






**Parameters:**


* `filename` 




        

<hr>



### function update\_from\_json 

_Update the scene from a scene commit json object._ 
```C++
void uipc::core::SceneIO::update_from_json (
    const Json & json
) 
```



Supported formats:
* - .json
* .bson






**Parameters:**


* `filename` 




        

<hr>



### function write\_surface 

_Write the surface of the scene to a file. Supported formats:_ 
```C++
void uipc::core::SceneIO::write_surface (
    std::string_view filename
) 
```




* .obj 




        

<hr>
## Public Static Functions Documentation




### function from\_json 

_Convert a json object to a scene._ 
```C++
static Scene uipc::core::SceneIO::from_json (
    const Json & json
) 
```





**Parameters:**


* `json` 



**Returns:**







        

<hr>



### function load 

_Load a scene from a file._ 
```C++
static Scene uipc::core::SceneIO::load (
    std::string_view filename
) 
```



Supported formats:
* .json
* .bson






**Parameters:**


* `filename` 



**Returns:**







        

<hr>



### function save [2/2]

_Save the scene to a file._ 
```C++
static void uipc::core::SceneIO::save (
    const Scene & scene,
    std::string_view filename
) 
```



Supported formats:
* .json
* .bson






**Parameters:**


* `scene` 
* `filename` 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/io/scene_io.h`

