

# File affine\_body\_state\_accessor\_feature.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**affine\_body\_state\_accessor\_feature.h**](affine__body__state__accessor__feature_8h.md)

[Go to the documentation of this file](affine__body__state__accessor__feature_8h.md)


```C++
#pragma once
#include <uipc/core/feature.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::core
{
class UIPC_CORE_API AffineBodyStateAccessorFeatureOverrider
{
  public:
    AffineBodyStateAccessorFeatureOverrider()          = default;
    virtual ~AffineBodyStateAccessorFeatureOverrider() = default;

    virtual SizeT get_body_count() = 0;
    virtual geometry::SimplicialComplex do_create_geometry(IndexT body_offset, SizeT body_count);
    virtual void do_copy_from(const geometry::SimplicialComplex& state_geo) = 0;
    virtual void do_copy_to(geometry::SimplicialComplex& state_geo)         = 0;
};

class UIPC_CORE_API AffineBodyStateAccessorFeature final : public Feature
{
  public:
    constexpr static std::string_view FeatureName = "core/affine_body_state_accessor";

    explicit AffineBodyStateAccessorFeature(S<AffineBodyStateAccessorFeatureOverrider> overrider);

    SizeT body_count() const;

    geometry::SimplicialComplex create_geometry(IndexT body_offset = 0,
                                                SizeT  body_count  = ~0ull);

    void copy_from(const geometry::SimplicialComplex& state_geo) const;

    void copy_to(geometry::SimplicialComplex& state_geo) const;

  private:
    virtual std::string_view                   get_name() const override;
    S<AffineBodyStateAccessorFeatureOverrider> m_impl;
};
}  // namespace uipc::core
```


