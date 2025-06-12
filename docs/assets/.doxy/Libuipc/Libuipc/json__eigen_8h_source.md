

# File json\_eigen.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**json\_eigen.h**](json__eigen_8h.md)

[Go to the documentation of this file](json__eigen_8h.md)


```C++
#pragma once
#include <nlohmann/adl_serializer.hpp>
#include <Eigen/Core>
#include <uipc/common/exception.h>

namespace uipc
{
class UIPC_CORE_API JsonIOError : public Exception
{
  public:
    using Exception::Exception;
};
}  // namespace uipc

namespace nlohmann
{
template <typename Scalar, int Rows, int Cols, int Options, int MaxRows, int MaxCols>
struct adl_serializer<Eigen::Matrix<Scalar, Rows, Cols, Options, MaxRows, MaxCols>>
{
    static void to_json(json& j,
                        const Eigen::Matrix<Scalar, Rows, Cols, Options, MaxRows, MaxCols>& m);

    static void from_json(const json& j,
                          Eigen::Matrix<Scalar, Rows, Cols, Options, MaxRows, MaxCols>& m);
};
}  // namespace nlohmann

#include "details/eigen_json.inl"
```


