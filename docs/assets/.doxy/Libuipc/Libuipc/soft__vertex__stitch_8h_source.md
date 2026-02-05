

# File soft\_vertex\_stitch.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**soft\_vertex\_stitch.h**](soft__vertex__stitch_8h.md)

[Go to the documentation of this file](soft__vertex__stitch_8h.md)


```C++
#pragma once
#include <uipc/constitution/inter_primitive_constitution.h>
#include <uipc/geometry/geometry.h>
#include <uipc/geometry/simplicial_complex_slot.h>
#include <uipc/core/contact_element.h>
namespace uipc::constitution
{
class UIPC_CONSTITUTION_API SoftVertexStitch final : public InterPrimitiveConstitution
{
    using Base = InterPrimitiveConstitution;

  public:
    using SlotTuple =
        std::tuple<S<geometry::SimplicialComplexSlot>, S<geometry::SimplicialComplexSlot>>;
    using ContactElementTuple = std::tuple<core::ContactElement, core::ContactElement>;

    SoftVertexStitch(const Json& config = default_config());

    geometry::Geometry create_geometry(const SlotTuple&     aim_geo_slots,
                                       span<const Vector2i> stitched_vert_ids,
                                       Float                kappa = 1e6,
                                       Float rest_length          = 0.0) const;


    geometry::Geometry create_geometry(const SlotTuple&     aim_geo_slots,
                                       span<const Vector2i> stitched_vert_ids,
                                       const ContactElementTuple& contact_elements,
                                       Float kappa       = 1e6,
                                       Float rest_length = 0.0) const;
    static Json        default_config();

  private:
    U64  get_uid() const noexcept override;
    Json m_config;
};
}  // namespace uipc::constitution
```


