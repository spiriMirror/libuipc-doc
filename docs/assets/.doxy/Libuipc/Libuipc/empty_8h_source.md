

# File empty.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**empty.h**](empty_8h.md)

[Go to the documentation of this file](empty_8h.md)


```C++
#pragma once
#include <uipc/constitution/finite_element_constitution.h>
#include <uipc/constitution/elastic_moduli.h>
#include <uipc/common/unit.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API Empty : public FiniteElementConstitution
{
    using Base = FiniteElementConstitution;

  public:
    Empty(const Json& config = default_config()) noexcept;

    void apply_to(geometry::SimplicialComplex& sc,
                  Float                        mass_density = 1000.0,
                  Float                        thickness    = 0.01_m) const;

    static Json default_config() noexcept;

  protected:
    virtual U64 get_uid() const noexcept override;

  private:
    Json m_config;
};
}  // namespace uipc::constitution
```


