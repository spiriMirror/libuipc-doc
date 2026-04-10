

# File finite\_element\_external\_force.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**finite\_element\_external\_force.h**](finite__element__external__force_8h.md)

[Go to the documentation of this file](finite__element__external__force_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/constitution/constitution.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API FiniteElementExternalForce final : public IConstitution
{
    using Base = IConstitution;

  public:
    FiniteElementExternalForce(const Json& config = default_config());
    ~FiniteElementExternalForce();

    void apply_to(geometry::SimplicialComplex& sc, const Vector3& force);

    static Json default_config();

  protected:
    virtual U64 get_uid() const noexcept override;

  private:
    Json m_config;
};
}  // namespace uipc::constitution
```


