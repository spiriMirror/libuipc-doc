

# File log.h



[**FileList**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**log.h**](log_8h.md)

[Go to the source code of this file](log_8h_source.md)



* `#include <spdlog/spdlog.h>`
* `#include <uipc/common/string.h>`
* `#include <uipc/common/config.h>`
* `#include <uipc/common/abort.h>`
































































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**UIPC\_ASSERT**](log_8h.md#define-uipc_assert) (condition, ...) `/* multi line expression */`<br> |
| define  | [**UIPC\_ERROR\_WITH\_LOCATION**](log_8h.md#define-uipc_error_with_location) (...) `UIPC\_LOG\_WITH\_LOCATION(spdlog::level::err, \_\_VA\_ARGS\_\_)`<br> |
| define  | [**UIPC\_INFO\_WITH\_LOCATION**](log_8h.md#define-uipc_info_with_location) (...) `UIPC\_LOG\_WITH\_LOCATION(spdlog::level::info, \_\_VA\_ARGS\_\_)`<br> |
| define  | [**UIPC\_LOG\_WITH\_LOCATION**](log_8h.md#define-uipc_log_with_location) (level, ...) `/* multi line expression */`<br> |
| define  | [**UIPC\_WARN\_WITH\_LOCATION**](log_8h.md#define-uipc_warn_with_location) (...) `UIPC\_LOG\_WITH\_LOCATION(spdlog::level::warn, \_\_VA\_ARGS\_\_)`<br> |

## Macro Definition Documentation





### define UIPC\_ASSERT 

```C++
#define UIPC_ASSERT (
    condition,
    ...
) `/* multi line expression */`
```




<hr>



### define UIPC\_ERROR\_WITH\_LOCATION 

```C++
#define UIPC_ERROR_WITH_LOCATION (
    ...
) `UIPC_LOG_WITH_LOCATION(spdlog::level::err, __VA_ARGS__)`
```




<hr>



### define UIPC\_INFO\_WITH\_LOCATION 

```C++
#define UIPC_INFO_WITH_LOCATION (
    ...
) `UIPC_LOG_WITH_LOCATION(spdlog::level::info, __VA_ARGS__)`
```




<hr>



### define UIPC\_LOG\_WITH\_LOCATION 

```C++
#define UIPC_LOG_WITH_LOCATION (
    level,
    ...
) `/* multi line expression */`
```




<hr>



### define UIPC\_WARN\_WITH\_LOCATION 

```C++
#define UIPC_WARN_WITH_LOCATION (
    ...
) `UIPC_LOG_WITH_LOCATION(spdlog::level::warn, __VA_ARGS__)`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/log.h`

