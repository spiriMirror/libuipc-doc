

# File soft\_position\_constraint.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**soft\_position\_constraint.h**](soft__position__constraint_8h.md)

[Go to the documentation of this file](soft__position__constraint_8h.md)


```C++
#pragma once
#include <uipc/constitution/constraint.h>
#include <uipc/geometry/simplicial_complex.h>
#include <uipc/common/json.h>
namespace uipc::constitution
{
class UIPC_CONSTITUTION_API SoftPositionConstraint final : public Constraint
{
    using Base = Constraint;

  public:
    SoftPositionConstraint(const Json& config = default_config()) noexcept;

    void apply_to(geometry::SimplicialComplex& sc, Float strength_rate = 100.0) const;

    static Json default_config();

  protected:
    U64 get_uid() const noexcept override;

  private:
    Json m_config;
};
}  // namespace uipc::constitution
```


