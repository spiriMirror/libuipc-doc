

# Class uipc::geometry::SimplicialComplexIO



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**SimplicialComplexIO**](classuipc_1_1geometry_1_1_simplicial_complex_i_o.md)



_A class for reading and writing simplicial complex._ 

* `#include <simplicial_complex_io.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SimplicialComplexIO**](#function-simplicialcomplexio-15) () = default<br> |
|   | [**SimplicialComplexIO**](#function-simplicialcomplexio-25) (const Matrix4x4 & pre\_transform) noexcept<br> |
|   | [**SimplicialComplexIO**](#function-simplicialcomplexio-35) (const Transform & pre\_transform) noexcept<br> |
|   | [**SimplicialComplexIO**](#function-simplicialcomplexio-45) (const [**SimplicialComplexIO**](classuipc_1_1geometry_1_1_simplicial_complex_i_o.md) &) = default<br> |
|   | [**SimplicialComplexIO**](#function-simplicialcomplexio-55) ([**SimplicialComplexIO**](classuipc_1_1geometry_1_1_simplicial_complex_i_o.md) &&) = default<br> |
|  [**SimplicialComplexIO**](classuipc_1_1geometry_1_1_simplicial_complex_i_o.md) & | [**operator=**](#function-operator) (const [**SimplicialComplexIO**](classuipc_1_1geometry_1_1_simplicial_complex_i_o.md) &) = default<br> |
|  [**SimplicialComplexIO**](classuipc_1_1geometry_1_1_simplicial_complex_i_o.md) & | [**operator=**](#function-operator_1) ([**SimplicialComplexIO**](classuipc_1_1geometry_1_1_simplicial_complex_i_o.md) &&) = default<br> |
|  [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**read**](#function-read) (std::string\_view file\_name) <br>_A unified interface for reading a simplicial complex from a file, the file type is determined by the file extension._  |
|  [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**read\_msh**](#function-read_msh) (std::string\_view file\_name) <br>_Read a tetmesh from a .msh file._  |
|  [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**read\_obj**](#function-read_obj) (std::string\_view file\_name) <br>_Read a trimesh, linemesh or particles from a .obj file._  |
|  [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**read\_ply**](#function-read_ply) (std::string\_view file\_name) <br>_Read a trimesh, linemesh or particles from a .ply file._  |
|  [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**read\_stl**](#function-read_stl) (std::string\_view file\_name) <br>_Read a trimesh, linemesh or particles from a .stl file._  |
|  void | [**write**](#function-write) (std::string\_view file\_name, const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc) <br>_Write a simplicial complex to a file, the file type is determined by the file extension._  |
|  void | [**write\_msh**](#function-write_msh) (std::string\_view file\_name, const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc) <br>_Write a simplicial complex to .msh file._  |
|  void | [**write\_obj**](#function-write_obj) (std::string\_view file\_name, const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & sc) <br>_Write a simplicial complex to .obj file._  |




























## Public Functions Documentation




### function SimplicialComplexIO [1/5]

```C++
uipc::geometry::SimplicialComplexIO::SimplicialComplexIO () = default
```




<hr>



### function SimplicialComplexIO [2/5]

```C++
explicit uipc::geometry::SimplicialComplexIO::SimplicialComplexIO (
    const Matrix4x4 & pre_transform
) noexcept
```




<hr>



### function SimplicialComplexIO [3/5]

```C++
explicit uipc::geometry::SimplicialComplexIO::SimplicialComplexIO (
    const Transform & pre_transform
) noexcept
```




<hr>



### function SimplicialComplexIO [4/5]

```C++
uipc::geometry::SimplicialComplexIO::SimplicialComplexIO (
    const SimplicialComplexIO &
) = default
```




<hr>



### function SimplicialComplexIO [5/5]

```C++
uipc::geometry::SimplicialComplexIO::SimplicialComplexIO (
    SimplicialComplexIO &&
) = default
```




<hr>



### function operator= 

```C++
SimplicialComplexIO & uipc::geometry::SimplicialComplexIO::operator= (
    const SimplicialComplexIO &
) = default
```




<hr>



### function operator= 

```C++
SimplicialComplexIO & uipc::geometry::SimplicialComplexIO::operator= (
    SimplicialComplexIO &&
) = default
```




<hr>



### function read 

_A unified interface for reading a simplicial complex from a file, the file type is determined by the file extension._ 
```C++
SimplicialComplex uipc::geometry::SimplicialComplexIO::read (
    std::string_view file_name
) 
```





**Parameters:**


* `file_name` The file to read 



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) 





        

<hr>



### function read\_msh 

_Read a tetmesh from a .msh file._ 
```C++
SimplicialComplex uipc::geometry::SimplicialComplexIO::read_msh (
    std::string_view file_name
) 
```





**Parameters:**


* `file_name` The file to read



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) 





        

<hr>



### function read\_obj 

_Read a trimesh, linemesh or particles from a .obj file._ 
```C++
SimplicialComplex uipc::geometry::SimplicialComplexIO::read_obj (
    std::string_view file_name
) 
```





**Parameters:**


* `file_name` The file to read



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) 





        

<hr>



### function read\_ply 

_Read a trimesh, linemesh or particles from a .ply file._ 
```C++
SimplicialComplex uipc::geometry::SimplicialComplexIO::read_ply (
    std::string_view file_name
) 
```





**Parameters:**


* `file_name` The file to read



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) 





        

<hr>



### function read\_stl 

_Read a trimesh, linemesh or particles from a .stl file._ 
```C++
SimplicialComplex uipc::geometry::SimplicialComplexIO::read_stl (
    std::string_view file_name
) 
```





**Parameters:**


* `file_name` The file to read



**Returns:**

[**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) 





        

<hr>



### function write 

_Write a simplicial complex to a file, the file type is determined by the file extension._ 
```C++
void uipc::geometry::SimplicialComplexIO::write (
    std::string_view file_name,
    const SimplicialComplex & sc
) 
```





**Parameters:**


* `file_name` The file to write 
* `sc` The simplicial complex to write 




        

<hr>



### function write\_msh 

_Write a simplicial complex to .msh file._ 
```C++
void uipc::geometry::SimplicialComplexIO::write_msh (
    std::string_view file_name,
    const SimplicialComplex & sc
) 
```





**Parameters:**


* `file_name` The file to write 
* `sc` The simplicial complex to write 




        

<hr>



### function write\_obj 

_Write a simplicial complex to .obj file._ 
```C++
void uipc::geometry::SimplicialComplexIO::write_obj (
    std::string_view file_name,
    const SimplicialComplex & sc
) 
```





**Parameters:**


* `file_name` The file to write 
* `sc` The simplicial complex to write 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/io/simplicial_complex_io.h`

