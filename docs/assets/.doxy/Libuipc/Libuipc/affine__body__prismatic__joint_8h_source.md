

# File affine\_body\_prismatic\_joint.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**affine\_body\_prismatic\_joint.h**](affine__body__prismatic__joint_8h.md)

[Go to the documentation of this file](affine__body__prismatic__joint_8h.md)


```C++
#pragma once
#include <uipc/constitution/inter_affine_body_constitution.h>
#include <uipc/geometry/simplicial_complex_slot.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API AffineBodyPrismaticJoint final : public InterAffineBodyConstitution
{
  public:
    using SlotTuple =
        std::tuple<S<geometry::SimplicialComplexSlot>, S<geometry::SimplicialComplexSlot>>;

    static Json default_config();

    AffineBodyPrismaticJoint(const Json& config = default_config());

    virtual ~AffineBodyPrismaticJoint();

    [[nodiscard]] geometry::SimplicialComplex create_geometry(
        span<const Vector3>                      position0s,
        span<const Vector3>                      position1s,
        span<S<geometry::SimplicialComplexSlot>> l_geo_slots,
        span<IndexT>                             l_instance_ids,
        span<S<geometry::SimplicialComplexSlot>> r_geo_slots,
        span<IndexT>                             r_instance_ids,
        span<Float>                              strength_ratios);

    [[nodiscard]] geometry::SimplicialComplex create_geometry(
        span<const Vector3>                      l_position0,
        span<const Vector3>                      l_position1,
        span<const Vector3>                      r_position0,
        span<const Vector3>                      r_position1,
        span<S<geometry::SimplicialComplexSlot>> l_geo_slots,
        span<IndexT>                             l_instance_ids,
        span<S<geometry::SimplicialComplexSlot>> r_geo_slots,
        span<IndexT>                             r_instance_ids,
        span<Float>                              strength_ratios);

    void apply_to(geometry::SimplicialComplex&             edges,
                  span<S<geometry::SimplicialComplexSlot>> l_geo_slots,
                  span<S<geometry::SimplicialComplexSlot>> r_geo_slots,
                  Float strength_ratio = Float{100});

    void apply_to(geometry::SimplicialComplex&             edges,
                  span<S<geometry::SimplicialComplexSlot>> l_geo_slots,
                  span<IndexT>                             l_instance_ids,
                  span<S<geometry::SimplicialComplexSlot>> r_geo_slots,
                  span<IndexT>                             r_instance_ids,
                  span<Float>                              strength_ratios);

  private:
    virtual U64 get_uid() const noexcept override;
    Json        m_config;
};
}  // namespace uipc::constitution
```


