

# File affine\_body\_spherical\_joint.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**affine\_body\_spherical\_joint.h**](affine__body__spherical__joint_8h.md)

[Go to the documentation of this file](affine__body__spherical__joint_8h.md)


```C++
#pragma once
#include <uipc/constitution/inter_affine_body_constitution.h>
#include <uipc/geometry/simplicial_complex_slot.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API AffineBodySphericalJoint final : public InterAffineBodyConstitution
{
  public:
    static Json default_config();

    AffineBodySphericalJoint(const Json& config = default_config());

    virtual ~AffineBodySphericalJoint();

    [[nodiscard]] geometry::SimplicialComplex create_geometry(
        span<const Vector3>                      positions,
        span<S<geometry::SimplicialComplexSlot>> l_geo_slots,
        span<IndexT>                             l_instance_ids,
        span<S<geometry::SimplicialComplexSlot>> r_geo_slots,
        span<IndexT>                             r_instance_ids,
        span<Float>                              strength_ratios);

    [[nodiscard]] geometry::SimplicialComplex create_geometry(
        span<const Vector3>                      l_positions,
        span<const Vector3>                      r_positions,
        span<S<geometry::SimplicialComplexSlot>> l_geo_slots,
        span<IndexT>                             l_instance_ids,
        span<S<geometry::SimplicialComplexSlot>> r_geo_slots,
        span<IndexT>                             r_instance_ids,
        span<Float>                              strength_ratios);

    void apply_to(geometry::SimplicialComplex&             sc,
                  span<S<geometry::SimplicialComplexSlot>> l_geo_slots,
                  span<S<geometry::SimplicialComplexSlot>> r_geo_slots,
                  Float strength_ratio = Float{100});

    void apply_to(geometry::SimplicialComplex&             sc,
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


