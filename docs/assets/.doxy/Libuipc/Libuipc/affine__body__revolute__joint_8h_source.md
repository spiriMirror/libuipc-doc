

# File affine\_body\_revolute\_joint.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**affine\_body\_revolute\_joint.h**](affine__body__revolute__joint_8h.md)

[Go to the documentation of this file](affine__body__revolute__joint_8h.md)


```C++
#pragma once
#include <uipc/constitution/inter_affine_body_constitution.h>
#include <uipc/geometry/simplicial_complex_slot.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API AffineBodyRevoluteJoint final : public InterAffineBodyConstitution
{
  public:
    using SlotTuple =
        std::tuple<S<geometry::SimplicialComplexSlot>, S<geometry::SimplicialComplexSlot>>;

    static Json default_config();

    AffineBodyRevoluteJoint(const Json& config = default_config());

    virtual ~AffineBodyRevoluteJoint();

    void apply_to(geometry::SimplicialComplex& edges,
                  span<SlotTuple>              geo_slots,
                  Float                        strength_ratio = Float{100});

  private:
    virtual U64 get_uid() const noexcept override;
    Json        m_config;
};
}  // namespace uipc::constitution
```


