

# File simplex\_utils.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**simplex\_utils.h**](simplex__utils_8h.md)

[Go to the documentation of this file](simplex__utils_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/common/dllexport.h>
#include <uipc/common/span.h>
namespace uipc::geometry
{
class UIPC_GEOMETRY_API SimplexUtils
{
  public:
    static bool is_same_edge(const Vector2i&, const Vector2i&) noexcept;
    static bool is_same_oriented_edge(const Vector2i&, const Vector2i&) noexcept;
    static bool is_same_tri(const Vector3i&, const Vector3i&) noexcept;
    static bool is_same_oriented_tri(const Vector3i&, const Vector3i&) noexcept;
    static bool is_same_tet(const Vector4i&, const Vector4i&) noexcept;
    static bool is_same_oriented_tet(const Vector4i&, const Vector4i&) noexcept;
    static bool compare_edge(const Vector2i&, const Vector2i&) noexcept;
    static bool compare_tri(const Vector3i&, const Vector3i&) noexcept;
    static bool compare_tet(const Vector4i&, const Vector4i&) noexcept;

    static void outward_tri_from_tet(span<const Vector3, 4> Vs, span<Vector3i, 4> Fs) noexcept;
};
}  // namespace uipc::geometry
```


