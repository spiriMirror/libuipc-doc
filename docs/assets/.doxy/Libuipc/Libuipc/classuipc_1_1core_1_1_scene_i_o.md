

# Class uipc::core::SceneIO



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SceneIO**](classuipc_1_1core_1_1_scene_i_o.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SceneIO**](#function-sceneio) ([**Scene**](classuipc_1_1core_1_1_scene.md) & scene) <br> |
|  [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**simplicial\_surface**](#function-simplicial_surface-12) () const<br> |
|  [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**simplicial\_surface**](#function-simplicial_surface-22) (IndexT dim) const<br> |
|  void | [**write\_surface**](#function-write_surface) (std::string\_view filename) <br> |




























## Public Functions Documentation




### function SceneIO 

```C++
uipc::core::SceneIO::SceneIO (
    Scene & scene
) 
```




<hr>



### function simplicial\_surface [1/2]

```C++
geometry::SimplicialComplex uipc::core::SceneIO::simplicial_surface () const
```




<hr>



### function simplicial\_surface [2/2]

```C++
geometry::SimplicialComplex uipc::core::SceneIO::simplicial_surface (
    IndexT dim
) const
```




<hr>



### function write\_surface 

```C++
void uipc::core::SceneIO::write_surface (
    std::string_view filename
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/io/scene_io.h`

