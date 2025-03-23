

# File span\_as\_eigen.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**span\_as\_eigen.h**](span__as__eigen_8h.md)

[Go to the documentation of this file](span__as__eigen_8h.md)


```C++
#pragma once
#include <Eigen/Core>
#include <uipc/common/span.h>

namespace uipc
{
template <std::floating_point T>
inline auto as_eigen(span<T> s)
{
    return Eigen::Map<Eigen::Matrix<T, Eigen::Dynamic, 1>>(s.data(), s.size());
}

template <std::floating_point T>
inline auto as_eigen(span<const T> s)
{
    return Eigen::Map<const Eigen::Matrix<T, Eigen::Dynamic, 1>>(s.data(), s.size());
}
}  // namespace uipc
```


