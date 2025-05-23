

# Class uipc::core::Engine



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**Engine**](classuipc_1_1core_1_1_engine.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Engine**](#function-engine-13) (std::string\_view backend\_name, std::string\_view workspace="./", const Json & config=default\_config()) <br> |
|   | [**Engine**](#function-engine-23) (const [**Engine**](classuipc_1_1core_1_1_engine.md) &) = delete<br> |
|   | [**Engine**](#function-engine-33) ([**Engine**](classuipc_1_1core_1_1_engine.md) &&) noexcept<br> |
|  std::string\_view | [**backend\_name**](#function-backend_name) () noexcept const<br> |
|  const [**FeatureCollection**](classuipc_1_1core_1_1_feature_collection.md) & | [**features**](#function-features) () <br> |
|  [**Engine**](classuipc_1_1core_1_1_engine.md) & | [**operator=**](#function-operator) (const [**Engine**](classuipc_1_1core_1_1_engine.md) &) = delete<br> |
|  [**Engine**](classuipc_1_1core_1_1_engine.md) & | [**operator=**](#function-operator_1) ([**Engine**](classuipc_1_1core_1_1_engine.md) &&) noexcept<br> |
|  [**EngineStatusCollection**](classuipc_1_1core_1_1_engine_status_collection.md) & | [**status**](#function-status) () <br> |
|  Json | [**to\_json**](#function-to_json) () const<br> |
|  std::string\_view | [**workspace**](#function-workspace) () noexcept const<br> |
|   | [**~Engine**](#function-engine) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Json | [**default\_config**](#function-default_config) () <br> |


























## Public Functions Documentation




### function Engine [1/3]

```C++
uipc::core::Engine::Engine (
    std::string_view backend_name,
    std::string_view workspace="./",
    const Json & config=default_config()
) 
```




<hr>



### function Engine [2/3]

```C++
uipc::core::Engine::Engine (
    const Engine &
) = delete
```




<hr>



### function Engine [3/3]

```C++
uipc::core::Engine::Engine (
    Engine &&
) noexcept
```




<hr>



### function backend\_name 

```C++
std::string_view uipc::core::Engine::backend_name () noexcept const
```




<hr>



### function features 

```C++
const FeatureCollection & uipc::core::Engine::features () 
```




<hr>



### function operator= 

```C++
Engine & uipc::core::Engine::operator= (
    const Engine &
) = delete
```




<hr>



### function operator= 

```C++
Engine & uipc::core::Engine::operator= (
    Engine &&
) noexcept
```




<hr>



### function status 

```C++
EngineStatusCollection & uipc::core::Engine::status () 
```




<hr>



### function to\_json 

```C++
Json uipc::core::Engine::to_json () const
```




<hr>



### function workspace 

```C++
std::string_view uipc::core::Engine::workspace () noexcept const
```




<hr>



### function ~Engine 

```C++
uipc::core::Engine::~Engine () 
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::core::Engine::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/engine.h`

