

# File soft\_transform\_constraint.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**soft\_transform\_constraint.h**](soft__transform__constraint_8h.md)

[Go to the documentation of this file](soft__transform__constraint_8h.md)


```C++
#pragma once
#include <uipc/constitution/constraint.h>
#include <uipc/geometry/simplicial_complex.h>
#include <uipc/common/json.h>
#include <numbers>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API SoftTransformConstraint final : public Constraint
{
    using Base = Constraint;

  public:
    SoftTransformConstraint(const Json& config = default_config()) noexcept;

    void apply_to(geometry::SimplicialComplex& sc, const Vector2& strength_ratio) const;

    static Json default_config();

  protected:
    U64 get_uid() const noexcept override;

  private:
    Json m_config;
};

class UIPC_CONSTITUTION_API RotatingMotor final : public Constraint
{
    using Base = Constraint;

  public:
    RotatingMotor(const Json& config = default_config()) noexcept;

    void apply_to(geometry::SimplicialComplex& sc,
                  Float                        strength_ratio = 100.0,
                  Vector3 motor_rot_axis = Vector3::UnitX(),
                  Float   motor_rot_vel  = 2 * std::numbers::pi) const;

    static Json default_config();

    static void animate(geometry::SimplicialComplex& sc, Float dt);

  protected:
    U64 get_uid() const noexcept override;

  private:
    Json m_config;
};

class UIPC_CONSTITUTION_API LinearMotor final : public Constraint
{
    using Base = Constraint;

  public:
    LinearMotor(const Json& config = default_config()) noexcept;

    void apply_to(geometry::SimplicialComplex& sc,
                  Float                        strength_ratio = 100.0,
                  Vector3                      motor_axis = -Vector3::UnitZ(),
                  Float                        motor_vel  = 1.0) const;

    static Json default_config();

    static void animate(geometry::SimplicialComplex& sc, Float dt);

  protected:
    U64 get_uid() const noexcept override;

  private:
    Json m_config;
};
}  // namespace uipc::constitution
```


