

# File abstract\_simplicial\_complex.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**abstract\_simplicial\_complex.h**](abstract__simplicial__complex_8h.md)

[Go to the documentation of this file](abstract__simplicial__complex_8h.md)


```C++
#pragma once
#include <uipc/geometry/simplicial_complex_attributes.h>
#include <uipc/geometry/geometry.h>

namespace uipc::geometry
{
class UIPC_CORE_API AbstractSimplicialComplex : public Geometry
{
    template <typename T>
    friend class AttributeFriend;

  public:
    using VertexAttributes  = SimplicialComplexAttributes<false, 0>;
    using CVertexAttributes = SimplicialComplexAttributes<true, 0>;
    using EdgeAttributes  = SimplicialComplexAttributes<false, 1>;
    using CEdgeAttributes = SimplicialComplexAttributes<true, 1>;
    using TriangleAttributes  = SimplicialComplexAttributes<false, 2>;
    using CTriangleAttributes = SimplicialComplexAttributes<true, 2>;
    using TetrahedronAttributes  = SimplicialComplexAttributes<false, 3>;
    using CTetrahedronAttributes = SimplicialComplexAttributes<true, 3>;

    AbstractSimplicialComplex()                                   = default;
    AbstractSimplicialComplex(const AbstractSimplicialComplex& o) = default;
    AbstractSimplicialComplex(AbstractSimplicialComplex&& o)      = default;

    AbstractSimplicialComplex& operator=(const AbstractSimplicialComplex& o) = delete;
    AbstractSimplicialComplex& operator=(AbstractSimplicialComplex&& o) = delete;

    [[nodiscard]] VertexAttributes  vertices() noexcept;
    [[nodiscard]] CVertexAttributes vertices() const noexcept;

    [[nodiscard]] EdgeAttributes  edges() noexcept;
    [[nodiscard]] CEdgeAttributes edges() const noexcept;


    [[nodiscard]] TriangleAttributes  triangles() noexcept;
    [[nodiscard]] CTriangleAttributes triangles() const noexcept;
    [[nodiscard]] TetrahedronAttributes  tetrahedra() noexcept;
    [[nodiscard]] CTetrahedronAttributes tetrahedra() const noexcept;

    [[nodiscard]] IndexT dim() const noexcept;


  protected:
    virtual std::string_view   get_type() const noexcept override;
    [[nodiscard]] virtual Json do_to_json() const override;

  private:
    friend struct fmt::formatter<AbstractSimplicialComplex>;
    AttributeCollection m_vertex_attributes;
    AttributeCollection m_edge_attributes;
    AttributeCollection m_triangle_attributes;
    AttributeCollection m_tetrahedron_attributes;
};
}  // namespace uipc::geometry

namespace fmt
{
template <>
struct UIPC_CORE_API formatter<uipc::geometry::AbstractSimplicialComplex>
    : formatter<string_view>
{
    appender format(const uipc::geometry::AbstractSimplicialComplex& c,
                    format_context&                                  ctx) const;
};
}  // namespace fmt
```


