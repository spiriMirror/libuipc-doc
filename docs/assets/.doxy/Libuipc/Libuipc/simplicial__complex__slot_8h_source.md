

# File simplicial\_complex\_slot.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**simplicial\_complex\_slot.h**](simplicial__complex__slot_8h.md)

[Go to the documentation of this file](simplicial__complex__slot_8h.md)


```C++
#pragma once
#include <uipc/geometry/geometry_slot.h>
#include <uipc/geometry/simplicial_complex.h>
namespace uipc::geometry
{
template <>
class UIPC_CORE_API GeometrySlotT<SimplicialComplex> : public GeometrySlot
{
  public:
    GeometrySlotT(IndexT id, const SimplicialComplex& simplicial_complex) noexcept;

    GeometrySlotT(const GeometrySlotT&)            = delete;
    GeometrySlotT(GeometrySlotT&&)                 = delete;
    GeometrySlotT& operator=(const GeometrySlotT&) = delete;
    GeometrySlotT& operator=(GeometrySlotT&&)      = delete;

    SimplicialComplex&       geometry() noexcept;
    const SimplicialComplex& geometry() const noexcept;

  protected:
    virtual Geometry&       get_geometry() noexcept override;
    virtual const Geometry& get_geometry() const noexcept override;
    virtual S<GeometrySlot> do_clone() const override;

  private:
    SimplicialComplex m_simplicial_complex;
};

using SimplicialComplexSlot = GeometrySlotT<SimplicialComplex>;
}  // namespace uipc::geometry

namespace std
{
extern template class std::shared_ptr<uipc::geometry::SimplicialComplexSlot>;
}
```


