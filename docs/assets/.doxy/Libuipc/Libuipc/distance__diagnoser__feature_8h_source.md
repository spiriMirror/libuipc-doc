

# File distance\_diagnoser\_feature.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**distance\_diagnoser\_feature.h**](distance__diagnoser__feature_8h.md)

[Go to the documentation of this file](distance__diagnoser__feature_8h.md)


```C++
#pragma once
#include <uipc/core/feature.h>
#include <uipc/geometry/geometry.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::core
{
class UIPC_CORE_API DistanceDiagnoserFeatureOverrider
{
  public:
    virtual ~DistanceDiagnoserFeatureOverrider() = default;

    virtual void do_compute_point_triangle_distance(
        geometry::Geometry&                R,
        const geometry::SimplicialComplex& points,
        const geometry::SimplicialComplex& triangles) = 0;

    virtual void do_compute_edge_edge_distance(
        geometry::Geometry&                R,
        const geometry::SimplicialComplex& edges_a,
        const geometry::SimplicialComplex& edges_b,
        const geometry::SimplicialComplex& rest_edges_a,
        const geometry::SimplicialComplex& rest_edges_b) = 0;

    virtual void do_compute_point_edge_distance(
        geometry::Geometry&                R,
        const geometry::SimplicialComplex& points,
        const geometry::SimplicialComplex& edges) = 0;

    virtual void do_compute_point_point_distance(
        geometry::Geometry&                R,
        const geometry::SimplicialComplex& points_a,
        const geometry::SimplicialComplex& points_b) = 0;
};

class UIPC_CORE_API DistanceDiagnoserFeature final : public Feature
{
  public:
    constexpr static std::string_view FeatureName = "core/distance_diagnoser";

    DistanceDiagnoserFeature(S<DistanceDiagnoserFeatureOverrider> overrider);

    void compute_point_triangle_distance(
        geometry::Geometry&                R,
        const geometry::SimplicialComplex& points,
        const geometry::SimplicialComplex& triangles);

    void compute_edge_edge_distance(
        geometry::Geometry&                R,
        const geometry::SimplicialComplex& edges_a,
        const geometry::SimplicialComplex& edges_b,
        const geometry::SimplicialComplex& rest_edges_a,
        const geometry::SimplicialComplex& rest_edges_b);

    void compute_point_edge_distance(
        geometry::Geometry&                R,
        const geometry::SimplicialComplex& points,
        const geometry::SimplicialComplex& edges);

    void compute_point_point_distance(
        geometry::Geometry&                R,
        const geometry::SimplicialComplex& points_a,
        const geometry::SimplicialComplex& points_b);

  private:
    virtual std::string_view             get_name() const override;
    S<DistanceDiagnoserFeatureOverrider> m_impl;
};
}  // namespace uipc::core
```


