

# File affine\_body\_external\_force.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**affine\_body\_external\_force.h**](affine__body__external__force_8h.md)

[Go to the documentation of this file](affine__body__external__force_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/constitution/constitution.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API AffineBodyExternalBodyForce final : public IConstitution
{
    using Base = IConstitution;

  public:
    AffineBodyExternalBodyForce(const Json& config = default_config());
    ~AffineBodyExternalBodyForce();

    void apply_to(geometry::SimplicialComplex& sc, const Vector12& force);

    void apply_to(geometry::SimplicialComplex& sc, const Vector3& force);

    static Json default_config();

  protected:
    virtual U64 get_uid() const noexcept override;

  private:
    Json m_config;
};
}  // namespace uipc::constitution
```


