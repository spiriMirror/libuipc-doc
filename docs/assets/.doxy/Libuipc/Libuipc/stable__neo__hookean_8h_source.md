

# File stable\_neo\_hookean.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**stable\_neo\_hookean.h**](stable__neo__hookean_8h.md)

[Go to the documentation of this file](stable__neo__hookean_8h.md)


```C++
#pragma once
#include <uipc/constitution/finite_element_constitution.h>
#include <uipc/constitution/elastic_moduli.h>
#include <uipc/common/unit.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API StableNeoHookean : public FiniteElementConstitution
{
    using Base = FiniteElementConstitution;

  public:
    StableNeoHookean(const Json& config = default_config()) noexcept;

    void apply_to(geometry::SimplicialComplex& sc,
                  const ElasticModuli& moduli = ElasticModuli::youngs_poisson(20.0_kPa, 0.49),
                  Float mass_density = 1e3) const;

    static Json default_config() noexcept;

  protected:
    virtual U64 get_uid() const noexcept override;

  private:
    Json m_config;
};
}  // namespace uipc::constitution
```


