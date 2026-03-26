

# File stress\_plastic\_discrete\_shell\_bending.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**stress\_plastic\_discrete\_shell\_bending.h**](stress__plastic__discrete__shell__bending_8h.md)

[Go to the documentation of this file](stress__plastic__discrete__shell__bending_8h.md)


```C++
#pragma once
#include <uipc/constitution/finite_element_extra_constitution.h>
#include <uipc/common/unit.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API StressPlasticDiscreteShellBending
    : public FiniteElementExtraConstitution
{
    using Base = FiniteElementExtraConstitution;

  public:
    StressPlasticDiscreteShellBending(const Json& json = default_config());

    void apply_to(geometry::SimplicialComplex& sc,
                  Float                        bending_stiffness,
                  Float                        yield_stress,
                  Float                        hardening_modulus = 0.0);

    static Json default_config();

  private:
    virtual U64 get_uid() const noexcept final override;
    Json        m_config;
};
}  // namespace uipc::constitution
```


