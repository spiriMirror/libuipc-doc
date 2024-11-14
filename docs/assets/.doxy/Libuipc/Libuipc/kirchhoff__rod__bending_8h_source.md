

# File kirchhoff\_rod\_bending.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**kirchhoff\_rod\_bending.h**](kirchhoff__rod__bending_8h.md)

[Go to the documentation of this file](kirchhoff__rod__bending_8h.md)


```C++
#pragma once
#include <uipc/constitution/finite_element_extra_constitution.h>
#include <uipc/common/unit.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API KirchhoffRodBending : public FiniteElementExtraConstitution
{
    using Base = FiniteElementExtraConstitution;

  public:
    KirchhoffRodBending(const Json& json = default_config());

    void apply_to(geometry::SimplicialComplex& sc, Float E = 100.0_MPa);

    static Json default_config();


  private:
    virtual U64 get_uid() const noexcept final override;
    Json        m_config;
};
}  // namespace uipc::constitution
```


