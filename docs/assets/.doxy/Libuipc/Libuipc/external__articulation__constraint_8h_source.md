

# File external\_articulation\_constraint.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**external\_articulation\_constraint.h**](external__articulation__constraint_8h.md)

[Go to the documentation of this file](external__articulation__constraint_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/constitution/constraint.h>
#include <uipc/geometry/geometry_slot.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API ExternalArticulationConstraint final : public Constraint
{
    using Base = Constraint;

  public:
    ExternalArticulationConstraint(const Json& config = default_config()) noexcept;

    ~ExternalArticulationConstraint();

    [[nodiscard]] geometry::Geometry create_geometry(span<S<const geometry::GeometrySlot>> joint_geos) const;

    [[nodiscard]] geometry::Geometry create_geometry(span<S<const geometry::GeometrySlot>> joint_geos,
                                                     span<IndexT> indices) const;

    static Json default_config();

  protected:
    virtual U64 get_uid() const noexcept override;

  private:
    Json m_config;
};
}  // namespace uipc::constitution
```


