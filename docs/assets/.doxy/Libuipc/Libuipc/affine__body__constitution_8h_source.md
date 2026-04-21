

# File affine\_body\_constitution.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**affine\_body\_constitution.h**](affine__body__constitution_8h.md)

[Go to the documentation of this file](affine__body__constitution_8h.md)


```C++
#pragma once
#include <uipc/constitution/constitution.h>
#include <uipc/geometry/simplicial_complex.h>
#include <uipc/common/unit.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API AffineBodyConstitution : public IConstitution
{
    using Base = IConstitution;

  public:
    AffineBodyConstitution(const Json& config = default_config()) noexcept;

    void apply_to(geometry::SimplicialComplex& sc, Float kappa, Float mass_density = 1e3) const;

    void apply_to(geometry::SimplicialComplex& sc,
                  Float                        kappa,
                  const Matrix12x12&           mass,
                  Float                        volume) const;

    [[nodiscard]] geometry::SimplicialComplex create_proxy(Float              kappa,
                                                           Float              mass,
                                                           const Vector3&     mass_center,
                                                           const Matrix3x3&   inertia,
                                                           Float              volume) const;

    [[nodiscard]] geometry::SimplicialComplex create_proxy(Float              kappa,
                                                           const Matrix12x12& abd_mass,
                                                           Float              volume) const;

    static Json default_config() noexcept;

  protected:
    virtual U64 get_uid() const noexcept override;

    void create_attributes(geometry::SimplicialComplex& sc,
                               Float                        kappa,
                               Float                        mass_density,
                               Float                        volume,
                               Float                        m,
                               const Vector3&               m_x_bar,
                               const Matrix3x3&             m_x_bar_x_bar) const;

  private:
    Json m_config;
};
}  // namespace uipc::constitution
```


