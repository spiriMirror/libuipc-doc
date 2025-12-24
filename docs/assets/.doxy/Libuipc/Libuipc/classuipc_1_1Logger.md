

# Class uipc::Logger



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**Logger**](classuipc_1_1Logger.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef spdlog::level::level\_enum | [**Level**](#typedef-level)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**critical**](#function-critical) (std::string\_view fmt, Args &&... args) <br> |
|  void | [**debug**](#function-debug) (std::string\_view fmt, Args &&... args) <br> |
|  void | [**error**](#function-error) (std::string\_view fmt, Args &&... args) <br> |
|  spdlog::level::level\_enum | [**get\_level**](#function-get_level) () const<br> |
|  void | [**info**](#function-info) (std::string\_view fmt, Args &&... args) <br> |
|  void | [**log**](#function-log) (Level level, std::string\_view fmt, Args &&... args) <br> |
|  void | [**set\_level**](#function-set_level) (spdlog::level::level\_enum level) <br> |
|  void | [**set\_pattern**](#function-set_pattern) (std::string\_view pattern) <br> |
|  void | [**warn**](#function-warn) (std::string\_view fmt, Args &&... args) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**Logger**](classuipc_1_1Logger.md) | [**create\_console\_logger**](#function-create_console_logger) (std::string\_view logger\_name, spdlog::sink\_ptr sink\_ptr=nullptr) <br> |
|  void | [**current\_logger**](#function-current_logger-12) ([**Logger**](classuipc_1_1Logger.md) logger) <br> |
|  [**Logger**](classuipc_1_1Logger.md) | [**current\_logger**](#function-current_logger-22) () <br> |


























## Public Types Documentation




### typedef Level 

```C++
using uipc::Logger::Level =  spdlog::level::level_enum;
```




<hr>
## Public Functions Documentation




### function critical 

```C++
template<typename... Args>
inline void uipc::Logger::critical (
    std::string_view fmt,
    Args &&... args
) 
```




<hr>



### function debug 

```C++
template<typename... Args>
inline void uipc::Logger::debug (
    std::string_view fmt,
    Args &&... args
) 
```




<hr>



### function error 

```C++
template<typename... Args>
inline void uipc::Logger::error (
    std::string_view fmt,
    Args &&... args
) 
```




<hr>



### function get\_level 

```C++
spdlog::level::level_enum uipc::Logger::get_level () const
```




<hr>



### function info 

```C++
template<typename... Args>
inline void uipc::Logger::info (
    std::string_view fmt,
    Args &&... args
) 
```




<hr>



### function log 

```C++
template<typename... Args>
inline void uipc::Logger::log (
    Level level,
    std::string_view fmt,
    Args &&... args
) 
```




<hr>



### function set\_level 

```C++
void uipc::Logger::set_level (
    spdlog::level::level_enum level
) 
```




<hr>



### function set\_pattern 

```C++
void uipc::Logger::set_pattern (
    std::string_view pattern
) 
```




<hr>



### function warn 

```C++
template<typename... Args>
inline void uipc::Logger::warn (
    std::string_view fmt,
    Args &&... args
) 
```




<hr>
## Public Static Functions Documentation




### function create\_console\_logger 

```C++
static Logger uipc::Logger::create_console_logger (
    std::string_view logger_name,
    spdlog::sink_ptr sink_ptr=nullptr
) 
```




<hr>



### function current\_logger [1/2]

```C++
static void uipc::Logger::current_logger (
    Logger logger
) 
```




<hr>



### function current\_logger [2/2]

```C++
static Logger uipc::Logger::current_logger () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/logger.h`

