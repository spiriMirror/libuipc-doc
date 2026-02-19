

# File affine\_body\_revolute\_joint\_limit.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**affine\_body\_revolute\_joint\_limit.h**](affine__body__revolute__joint__limit_8h.md)

[Go to the documentation of this file](affine__body__revolute__joint__limit_8h.md)


```C++
#pragma once
#include <uipc/constitution/inter_affine_body_extra_constitution.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API AffineBodyRevoluteJointLimit final : public InterAffineBodyExtraConstitution
{
    using Base = InterAffineBodyExtraConstitution;

  public:
    AffineBodyRevoluteJointLimit(const Json& config = default_config());
    ~AffineBodyRevoluteJointLimit() override;

    void apply_to(geometry::SimplicialComplex& sc,
                  Float                        lower,
                  Float                        upper,
                  Float                        strength = 1.0f);

    void apply_to(geometry::SimplicialComplex& sc,
                  span<Float>                  lowers,
                  span<Float>                  uppers,
                  span<Float>                  strengths);

    static Json default_config();

  private:
    U64 get_uid() const noexcept override;
    Json m_config;
};
}  // namespace uipc::constitution
```


