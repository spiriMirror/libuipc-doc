

# Namespace uipc::logger



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**logger**](namespaceuipc_1_1logger.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**critical**](#function-critical) (std::string\_view fmt, Args &&... args) <br> |
|  void | [**debug**](#function-debug) (std::string\_view fmt, Args &&... args) <br> |
|  void | [**error**](#function-error) (std::string\_view fmt, Args &&... args) <br> |
|  UIPC\_CORE\_API Logger::Level | [**get\_level**](#function-get_level) () <br> |
|  void | [**info**](#function-info) (std::string\_view fmt, Args &&... args) <br> |
|  void | [**log**](#function-log) (Logger::Level level, std::string\_view fmt, Args &&... args) <br> |
|  UIPC\_CORE\_API void | [**set\_level**](#function-set_level) (Logger::Level level) <br> |
|  UIPC\_CORE\_API void | [**set\_pattern**](#function-set_pattern) (std::string\_view pattern) <br> |
|  void | [**warn**](#function-warn) (std::string\_view fmt, Args &&... args) <br> |




























## Public Functions Documentation




### function critical 

```C++
template<typename... Args>
inline void uipc::logger::critical (
    std::string_view fmt,
    Args &&... args
) 
```




<hr>



### function debug 

```C++
template<typename... Args>
inline void uipc::logger::debug (
    std::string_view fmt,
    Args &&... args
) 
```




<hr>



### function error 

```C++
template<typename... Args>
inline void uipc::logger::error (
    std::string_view fmt,
    Args &&... args
) 
```




<hr>



### function get\_level 

```C++
UIPC_CORE_API Logger::Level uipc::logger::get_level () 
```




<hr>



### function info 

```C++
template<typename... Args>
inline void uipc::logger::info (
    std::string_view fmt,
    Args &&... args
) 
```




<hr>



### function log 

```C++
template<typename... Args>
inline void uipc::logger::log (
    Logger::Level level,
    std::string_view fmt,
    Args &&... args
) 
```




<hr>



### function set\_level 

```C++
UIPC_CORE_API void uipc::logger::set_level (
    Logger::Level level
) 
```




<hr>



### function set\_pattern 

```C++
UIPC_CORE_API void uipc::logger::set_pattern (
    std::string_view pattern
) 
```




<hr>



### function warn 

```C++
template<typename... Args>
inline void uipc::logger::warn (
    std::string_view fmt,
    Args &&... args
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/logger.h`

