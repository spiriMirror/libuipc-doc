

# File strain\_plastic\_discrete\_shell\_bending.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**strain\_plastic\_discrete\_shell\_bending.h**](strain__plastic__discrete__shell__bending_8h.md)

[Go to the documentation of this file](strain__plastic__discrete__shell__bending_8h.md)


```C++
#pragma once
#include <uipc/constitution/finite_element_extra_constitution.h>
#include <uipc/common/unit.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API StrainPlasticDiscreteShellBending : public FiniteElementExtraConstitution
{
    using Base = FiniteElementExtraConstitution;

  public:
    StrainPlasticDiscreteShellBending(const Json& json = default_config());

    void apply_to(geometry::SimplicialComplex& sc,
                  Float                        bending_stiffness,
                  Float                        yield_threshold,
                  Float                        hardening_modulus = 0.0);

    static Json default_config();

  private:
    virtual U64 get_uid() const noexcept final override;
    Json        m_config;
};
}  // namespace uipc::constitution
```


