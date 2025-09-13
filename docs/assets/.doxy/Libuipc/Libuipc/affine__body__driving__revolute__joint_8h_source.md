

# File affine\_body\_driving\_revolute\_joint.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**affine\_body\_driving\_revolute\_joint.h**](affine__body__driving__revolute__joint_8h.md)

[Go to the documentation of this file](affine__body__driving__revolute__joint_8h.md)


```C++
#pragma once
#include <uipc/constitution/constraint.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API AffineBodyDrivingRevoluteJoint final : public Constraint
{
    using Base = Constraint;

  public:
    AffineBodyDrivingRevoluteJoint(const Json& config = default_config());

    ~AffineBodyDrivingRevoluteJoint() override;

    void apply_to(geometry::SimplicialComplex& sc, Float strength_ratio = Float{100});

    static Json default_config();

  private:
    virtual U64 get_uid() const noexcept override;
    Json        m_config;
};
}  // namespace uipc::constitution
```


