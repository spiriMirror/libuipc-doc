

# File flag.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**flag.h**](flag_8h.md)

[Go to the documentation of this file](flag_8h.md)


```C++
#pragma once
#include <concepts>
#include <type_traits>
#include <magic_enum/magic_enum.hpp>
#include <magic_enum/magic_enum_flags.hpp>

namespace uipc
{
template <typename T>
    requires std::is_enum_v<T>
constexpr auto to_underlying(const T& e) noexcept
{
    return static_cast<std::underlying_type_t<T>>(e);
}

template <typename T>
    requires std::is_enum_v<T>
constexpr bool has_flags(const T& flags, const T& test_flags) noexcept
{
    using namespace magic_enum::bitwise_operators;
    return (flags & test_flags) == test_flags;
}

template <typename T>
    requires std::is_enum_v<T>
constexpr bool is_valid_flag(const T& flag) noexcept
{
    auto value = to_underlying(flag);
    return value != 0 && (value & (value - 1)) == 0;
}
}  // namespace uipc
```


