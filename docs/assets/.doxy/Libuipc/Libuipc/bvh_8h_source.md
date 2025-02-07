

# File bvh.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**utils**](dir_739799d2da88efedfd4a7c44220c72e4.md) **>** [**bvh.h**](bvh_8h.md)

[Go to the documentation of this file](bvh_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/type_define.h>
#include <uipc/common/span.h>
#include <uipc/common/smart_pointer.h>
#include <Eigen/Geometry>

namespace uipc::geometry
{
class UIPC_GEOMETRY_API BVH
{
  public:
    using AABB = Eigen::AlignedBox<Float, 3>;

    BVH();
    ~BVH();

    void build(span<const AABB> aabbs);

    void clear();

    void query(span<const AABB> aabbs, std::function<void(IndexT, IndexT)>&& QF) const;
    
  private:
    class Impl;
    U<Impl> m_impl;
};
}  // namespace uipc::geometry
```


