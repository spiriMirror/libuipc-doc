

# File strain\_limiting\_baraff\_witkin.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**strain\_limiting\_baraff\_witkin.h**](strain__limiting__baraff__witkin_8h.md)

[Go to the documentation of this file](strain__limiting__baraff__witkin_8h.md)


```C++
#pragma once
#include <uipc/constitution/finite_element_constitution.h>
#include <uipc/constitution/elastic_moduli.h>
#include <uipc/common/unit.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API StrainLimitingBaraffWitkinShell : public FiniteElementConstitution
{
    using Base = FiniteElementConstitution;

  public:
    StrainLimitingBaraffWitkinShell(const Json& config = default_config()) noexcept;

    void apply_to(geometry::SimplicialComplex& sc,
                  const ElasticModuli& moduli = ElasticModuli::youngs_poisson(1.0_MPa, 0.49),
                  Float mass_density = 2e2,
                  Float thickness    = 0.001_m) const;

    static Json default_config() noexcept;

  protected:
    virtual U64 get_uid() const noexcept override;

  private:
    Json m_config;
};
}  // namespace uipc::constitution
```


