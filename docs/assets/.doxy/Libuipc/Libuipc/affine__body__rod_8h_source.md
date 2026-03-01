

# File affine\_body\_rod.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**affine\_body\_rod.h**](affine__body__rod_8h.md)

[Go to the documentation of this file](affine__body__rod_8h.md)


```C++
#pragma once
#include <uipc/constitution/affine_body_constitution.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API AffineBodyRod : public AffineBodyConstitution
{
  public:
    AffineBodyRod(const Json& config = default_config()) noexcept;

    void apply_to(geometry::SimplicialComplex& sc,
                  Float                        kappa,
                  Float                        mass_density = 1e3,
                  Float                        thickness    = 0.01) const;
};
}  // namespace uipc::constitution



```


