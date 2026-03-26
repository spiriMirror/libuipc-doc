

# File affine\_body\_revolute\_joint\_external\_force.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**affine\_body\_revolute\_joint\_external\_force.h**](affine__body__revolute__joint__external__force_8h.md)

[Go to the documentation of this file](affine__body__revolute__joint__external__force_8h.md)


```C++
#pragma once
#include <uipc/constitution/constraint.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API AffineBodyRevoluteJointExternalForce final : public Constraint
{
    using Base = Constraint;

  public:
    AffineBodyRevoluteJointExternalForce(const Json& config = default_config());

    ~AffineBodyRevoluteJointExternalForce() override;

    void apply_to(geometry::SimplicialComplex& sc, Float torque = Float{0});

    void apply_to(geometry::SimplicialComplex& sc, span<Float> torques);

    static Json default_config();

  private:
    virtual U64 get_uid() const noexcept override;
    Json        m_config;
};
}  // namespace uipc::constitution
```


