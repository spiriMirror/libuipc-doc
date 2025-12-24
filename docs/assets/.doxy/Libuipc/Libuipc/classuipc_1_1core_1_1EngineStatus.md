

# Class uipc::core::EngineStatus



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**EngineStatus**](classuipc_1_1core_1_1EngineStatus.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| enum int | [**Type**](#enum-type)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**EngineStatus**](#function-enginestatus) () = default<br> |
|  Type | [**type**](#function-type) () noexcept const<br> |
|  std::string\_view | [**what**](#function-what) () noexcept const<br> |
|   | [**~EngineStatus**](#function-enginestatus) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**EngineStatus**](classuipc_1_1core_1_1EngineStatus.md) | [**error**](#function-error) (std::string\_view msg) <br> |
|  [**EngineStatus**](classuipc_1_1core_1_1EngineStatus.md) | [**info**](#function-info) (std::string\_view msg) <br> |
|  [**EngineStatus**](classuipc_1_1core_1_1EngineStatus.md) | [**warning**](#function-warning) (std::string\_view msg) <br> |


























## Public Types Documentation




### enum Type 

```C++
enum uipc::core::EngineStatus::Type {
    None,
    Info,
    Warning,
    Error
};
```




<hr>
## Public Functions Documentation




### function EngineStatus 

```C++
uipc::core::EngineStatus::EngineStatus () = default
```




<hr>



### function type 

```C++
Type uipc::core::EngineStatus::type () noexcept const
```




<hr>



### function what 

```C++
std::string_view uipc::core::EngineStatus::what () noexcept const
```




<hr>



### function ~EngineStatus 

```C++
uipc::core::EngineStatus::~EngineStatus () = default
```




<hr>
## Public Static Functions Documentation




### function error 

```C++
static EngineStatus uipc::core::EngineStatus::error (
    std::string_view msg
) 
```




<hr>



### function info 

```C++
static EngineStatus uipc::core::EngineStatus::info (
    std::string_view msg
) 
```




<hr>



### function warning 

```C++
static EngineStatus uipc::core::EngineStatus::warning (
    std::string_view msg
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/engine_status.h`

