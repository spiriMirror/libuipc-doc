

# File simplicial\_complex.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**simplicial\_complex.h**](simplicial__complex_8h.md)

[Go to the documentation of this file](simplicial__complex_8h.md)


```C++
#pragma once
#include <uipc/geometry/geometry.h>
#include <uipc/geometry/abstract_simplicial_complex.h>
#include <uipc/geometry/simplicial_complex_attributes.h>

namespace uipc::geometry
{
class UIPC_CORE_API SimplicialComplex : public Geometry
{
    friend struct fmt::formatter<SimplicialComplex>;

    template <typename T>
    friend class AttributeFriend;

    template <typename T>
    friend class GeometryFriend;

  public:
    using VertexAttributes  = SimplicialComplexAttributes<false, 0>;
    using CVertexAttributes = SimplicialComplexAttributes<true, 0>;
    using EdgeAttributes  = SimplicialComplexAttributes<false, 1>;
    using CEdgeAttributes = SimplicialComplexAttributes<true, 1>;
    using TriangleAttributes  = SimplicialComplexAttributes<false, 2>;
    using CTriangleAttributes = SimplicialComplexAttributes<true, 2>;
    using TetrahedronAttributes  = SimplicialComplexAttributes<false, 3>;
    using CTetrahedronAttributes = SimplicialComplexAttributes<true, 3>;

    SimplicialComplex();


    SimplicialComplex(const SimplicialComplex& o) = default;
    SimplicialComplex(SimplicialComplex&& o)      = default;

    SimplicialComplex& operator=(const SimplicialComplex& o) = delete;
    SimplicialComplex& operator=(SimplicialComplex&& o)      = delete;


    [[nodiscard]] AttributeSlot<Matrix4x4>& transforms();
    [[nodiscard]] const AttributeSlot<Matrix4x4>& transforms() const;

    [[nodiscard]] AttributeSlot<Vector3>& positions() noexcept;

    [[nodiscard]] const AttributeSlot<Vector3>& positions() const noexcept;

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
    void do_collect_attribute_collections(vector<std::string>& names,
                                          vector<AttributeCollection*>& collections) override;

  private:
    AttributeCollection m_vertex_attributes;
    AttributeCollection m_edge_attributes;
    AttributeCollection m_triangle_attributes;
    AttributeCollection m_tetrahedron_attributes;
};
}  // namespace uipc::geometry

//formatter

namespace fmt
{
template <>
struct UIPC_CORE_API formatter<uipc::geometry::SimplicialComplex> : formatter<string_view>
{
    appender format(const uipc::geometry::SimplicialComplex& c, format_context& ctx) const;
};
}  // namespace fmt
```


