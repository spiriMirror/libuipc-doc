

# File finite\_element\_state\_accessor\_feature.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**finite\_element\_state\_accessor\_feature.h**](finite__element__state__accessor__feature_8h.md)

[Go to the documentation of this file](finite__element__state__accessor__feature_8h.md)


```C++
#pragma once
#include <uipc/core/feature.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::core
{
class UIPC_CORE_API FiniteElementStateAccessorFeatureOverrider
{
  public:
    virtual ~FiniteElementStateAccessorFeatureOverrider() = default;

    virtual SizeT                       get_vertex_count() = 0;
    virtual geometry::SimplicialComplex do_create_geometry(IndexT vertex_offset,
                                                           SizeT  vertex_count);
    virtual void do_copy_from(const geometry::SimplicialComplex& state_geo) = 0;
    virtual void do_copy_to(geometry::SimplicialComplex& state_geo)         = 0;
};

class UIPC_CORE_API FiniteElementStateAccessorFeature final : public Feature
{
  public:
    constexpr static std::string_view FeatureName = "core/finite_element_state_accessor";

    explicit FiniteElementStateAccessorFeature(S<FiniteElementStateAccessorFeatureOverrider> overrider);

    SizeT vertex_count() const;

    geometry::SimplicialComplex create_geometry(IndexT vertex_offset = 0,
                                                SizeT vertex_count = ~0ull) const;

    void copy_from(const geometry::SimplicialComplex& state_geo) const;

    void copy_to(geometry::SimplicialComplex& state_geo) const;

  private:
    virtual std::string_view                      get_name() const override;
    S<FiniteElementStateAccessorFeatureOverrider> m_impl;
};
}  // namespace uipc::core
```


