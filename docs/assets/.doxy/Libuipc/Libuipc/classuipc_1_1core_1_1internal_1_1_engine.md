

# Class uipc::core::internal::Engine



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**internal**](namespaceuipc_1_1core_1_1internal.md) **>** [**Engine**](classuipc_1_1core_1_1internal_1_1_engine.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Engine**](#function-engine) (std::string\_view backend\_name, std::string\_view workspace="./", const Json & config=default\_config()) <br> |
|  std::string\_view | [**backend\_name**](#function-backend_name) () noexcept const<br> |
|  const [**FeatureCollection**](classuipc_1_1core_1_1_feature_collection.md) & | [**features**](#function-features) () <br> |
|  [**EngineStatusCollection**](classuipc_1_1core_1_1_engine_status_collection.md) & | [**status**](#function-status) () <br> |
|  Json | [**to\_json**](#function-to_json) () const<br> |
|  std::string\_view | [**workspace**](#function-workspace) () noexcept const<br> |
|   | [**~Engine**](#function-engine) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Json | [**default\_config**](#function-default_config) () <br> |


























## Public Functions Documentation




### function Engine 

```C++
uipc::core::internal::Engine::Engine (
    std::string_view backend_name,
    std::string_view workspace="./",
    const Json & config=default_config()
) 
```




<hr>



### function backend\_name 

```C++
std::string_view uipc::core::internal::Engine::backend_name () noexcept const
```




<hr>



### function features 

```C++
const FeatureCollection & uipc::core::internal::Engine::features () 
```




<hr>



### function status 

```C++
EngineStatusCollection & uipc::core::internal::Engine::status () 
```




<hr>



### function to\_json 

```C++
Json uipc::core::internal::Engine::to_json () const
```




<hr>



### function workspace 

```C++
std::string_view uipc::core::internal::Engine::workspace () noexcept const
```




<hr>



### function ~Engine 

```C++
uipc::core::internal::Engine::~Engine () 
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::core::internal::Engine::default_config () 
```




<hr>## Friends Documentation





### friend World 

```C++
class uipc::core::internal::Engine::World (
    internal::World
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/internal/engine.h`

