

# Class uipc::io::UrdfIO



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**io**](namespaceuipc_1_1io.md) **>** [**UrdfIO**](classuipc_1_1io_1_1UrdfIO.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**UrdfIO**](#function-urdfio) (const Json & config=UrdfIO::default\_config()) <br> |
|  [**UrdfController**](classuipc_1_1io_1_1UrdfController.md) | [**read**](#function-read) ([**uipc::core::Object**](classuipc_1_1core_1_1Object.md) & object, std::string\_view urdf\_path) <br> |
|   | [**~UrdfIO**](#function-urdfio) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Json | [**default\_config**](#function-default_config) () <br> |


























## Public Functions Documentation




### function UrdfIO 

```C++
uipc::io::UrdfIO::UrdfIO (
    const Json & config=UrdfIO::default_config()
) 
```




<hr>



### function read 

```C++
UrdfController uipc::io::UrdfIO::read (
    uipc::core::Object & object,
    std::string_view urdf_path
) 
```




<hr>



### function ~UrdfIO 

```C++
uipc::io::UrdfIO::~UrdfIO () 
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::io::UrdfIO::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/io/urdf_io.h`

