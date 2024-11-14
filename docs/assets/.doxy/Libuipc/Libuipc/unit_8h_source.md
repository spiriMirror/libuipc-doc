

# File unit.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**unit.h**](unit_8h.md)

[Go to the documentation of this file](unit_8h.md)


```C++
#pragma once

namespace uipc
{
constexpr long double operator""_s(long double value)
{
    return value;
}

constexpr long double operator""_ms(long double value)
{
    return value * 1e-3;
}
constexpr long double operator""_m(long double value)
{
    return value;
}

constexpr long double operator""_mm(long double value)
{
    return value * 1e-3;
}

constexpr long double operator""_km(long double value)
{
    return value * 1e3;
}

constexpr long double operator""_Pa(long double value)
{
    return value;
}

constexpr long double operator""_kPa(long double value)
{
    return value * 1e3;
}

constexpr long double operator""_MPa(long double value)
{
    return value * 1e6;
}

constexpr long double operator""_GPa(long double value)
{
    return value * 1e9;
}

constexpr long double operator""_N(long double value)
{
    return value;
}
}  // namespace uipc
```


