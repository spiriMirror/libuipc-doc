

# File implicit\_geometry.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**implicit\_geometry.h**](implicit__geometry_8h.md)

[Go to the documentation of this file](implicit__geometry_8h.md)


```C++
#pragma once
#include <uipc/geometry/geometry.h>
#include <uipc/builtin/uid_info.h>
namespace uipc::geometry
{
class UIPC_CORE_API ImplicitGeometry : public Geometry
{
  public:
    ImplicitGeometry();

    const builtin::UIDInfo& uid_info() const noexcept;
    std::string_view        name() const noexcept;

  protected:
    std::string_view get_type() const noexcept override;
};
}  // namespace uipc::geometry

namespace fmt
{
template <>
struct UIPC_CORE_API formatter<uipc::geometry::ImplicitGeometry>
    : public formatter<std::string_view>
{
    appender format(const uipc::geometry::ImplicitGeometry& geometry,
                    format_context&                         ctx) const;
};
}  // namespace fmt
```


