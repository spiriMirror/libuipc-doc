

# Class uipc::core::SceneIO



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SceneIO**](classuipc_1_1core_1_1_scene_i_o.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SceneIO**](#function-sceneio) ([**Scene**](classuipc_1_1core_1_1_scene.md) & scene) <br> |
|  void | [**save**](#function-save-12) (std::string\_view filename) const<br>_Save the scene to a file._  |
|  [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**simplicial\_surface**](#function-simplicial_surface) (IndexT dim=-1) const<br>_Get the surface of the scene in the form of a simplicial complex allow to specify the dimension of the surface._  |
|  void | [**write\_surface**](#function-write_surface) (std::string\_view filename) <br>_Write the surface of the scene to a file. Supported formats:_  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  S&lt; [**Scene**](classuipc_1_1core_1_1_scene.md) &gt; | [**load**](#function-load) (std::string\_view filename) <br>_Load a scene from a file._  |
|  void | [**save**](#function-save-22) (const [**Scene**](classuipc_1_1core_1_1_scene.md) & scene, std::string\_view filename) <br>_Save the scene to a file._  |


























## Public Functions Documentation




### function SceneIO 

```C++
uipc::core::SceneIO::SceneIO (
    Scene & scene
) 
```




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




### function load 

_Load a scene from a file._ 
```C++
static S< Scene > uipc::core::SceneIO::load (
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

