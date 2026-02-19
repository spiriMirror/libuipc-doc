

# File affine\_body\_prismatic\_joint\_limit.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**affine\_body\_prismatic\_joint\_limit.h**](affine__body__prismatic__joint__limit_8h.md)

[Go to the documentation of this file](affine__body__prismatic__joint__limit_8h.md)


```C++
#pragma once
#include <uipc/constitution/inter_affine_body_extra_constitution.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API AffineBodyPrismaticJointLimit final : public InterAffineBodyExtraConstitution
{
    using Base = InterAffineBodyExtraConstitution;

  public:
    AffineBodyPrismaticJointLimit(const Json& config = default_config());
    ~AffineBodyPrismaticJointLimit() override;

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


