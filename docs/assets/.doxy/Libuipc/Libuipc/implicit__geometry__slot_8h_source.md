

# File implicit\_geometry\_slot.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**implicit\_geometry\_slot.h**](implicit__geometry__slot_8h.md)

[Go to the documentation of this file](implicit__geometry__slot_8h.md)


```C++
#pragma once
#include <uipc/geometry/geometry_slot.h>
#include <uipc/geometry/implicit_geometry.h>

namespace uipc::geometry
{
template <>
class UIPC_CORE_API GeometrySlotT<ImplicitGeometry> : public GeometrySlot
{
  public:
    GeometrySlotT(IndexT id, const ImplicitGeometry& geometry);

    ImplicitGeometry&       geometry() noexcept;
    const ImplicitGeometry& geometry() const noexcept;

  protected:
    Geometry&       get_geometry() noexcept override;
    const Geometry& get_geometry() const noexcept override;
    S<GeometrySlot> do_clone() const override;

  private:
    ImplicitGeometry m_geometry;
};

using ImplicitGeometrySlot = GeometrySlotT<ImplicitGeometry>;
}  // namespace uipc::geometry

namespace std
{
extern template class std::shared_ptr<uipc::geometry::ImplicitGeometrySlot>;
}
```


