

# File log.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**log.h**](log_8h.md)

[Go to the documentation of this file](log_8h.md)


```C++
#pragma once
#include <uipc/common/logger.h>
#include <uipc/common/string.h>
#include <uipc/common/config.h>
#include <uipc/common/abort.h>


#define UIPC_LOG_WITH_LOCATION(level, ...)                                     \
    {                                                                          \
        ::uipc::string msg = ::fmt::format(__VA_ARGS__);                       \
        ::uipc::logger::log((level), "{} {}({})", msg, __FILE__, __LINE__);       \
    }

#define UIPC_INFO_WITH_LOCATION(...)                                           \
    UIPC_LOG_WITH_LOCATION(spdlog::level::info, __VA_ARGS__)

#define UIPC_WARN_WITH_LOCATION(...)                                           \
    UIPC_LOG_WITH_LOCATION(spdlog::level::warn, __VA_ARGS__)

#define UIPC_ERROR_WITH_LOCATION(...)                                          \
    UIPC_LOG_WITH_LOCATION(spdlog::level::err, __VA_ARGS__)

#define UIPC_ASSERT(condition, ...)                                                            \
    {                                                                                          \
        if(!(condition))                                                                       \
        {                                                                                      \
            ::uipc::string msg = ::fmt::format(__VA_ARGS__);                                   \
            ::uipc::string assert_msg =                                                        \
                ::fmt::format("Assertion " #condition " failed. {}", msg);                     \
            ::uipc::logger::log(spdlog::level::err, "{} {}({})", assert_msg, __FILE__, __LINE__); \
            ::uipc::abort();                                                                   \
        }                                                                                      \
    }
```


