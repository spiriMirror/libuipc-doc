

# File arap.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**arap.h**](arap_8h.md)

[Go to the documentation of this file](arap_8h.md)


```C++
#pragma once
#include <uipc/constitution/finite_element_constitution.h>
#include <uipc/common/unit.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API ARAP : public FiniteElementConstitution
{
    using Base = FiniteElementConstitution;

  public:
    ARAP(const Json& config = default_config()) noexcept;

    void apply_to(geometry::SimplicialComplex& sc, Float kappa = 1.0_MPa, Float mass_density = 1e3) const;

    static Json default_config() noexcept;

  protected:
    virtual U64              get_uid() const noexcept override;

  private:
    Json m_config;
};
}  // namespace uipc::constitution
```


