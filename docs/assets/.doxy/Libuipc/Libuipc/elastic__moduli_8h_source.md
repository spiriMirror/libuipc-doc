

# File elastic\_moduli.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**elastic\_moduli.h**](elastic__moduli_8h.md)

[Go to the documentation of this file](elastic__moduli_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/type_define.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API ElasticModuli
{
  public:
    static ElasticModuli lame(Float lambda, Float mu) noexcept;
    static ElasticModuli youngs_shear(Float E, Float G) noexcept;
    static ElasticModuli youngs_poisson(Float E, Float nu);

    auto lambda() const noexcept { return m_lambda; }
    auto mu() const noexcept { return m_mu; }

  private:
    ElasticModuli() = default;
    ElasticModuli(Float lambda, Float mu) noexcept;
    Float m_lambda;
    Float m_mu;
};

class UIPC_CONSTITUTION_API ElasticModuli2D
{
  public:
    static ElasticModuli2D lame(Float lambda, Float mu) noexcept;
    static ElasticModuli2D youngs_shear(Float E, Float G) noexcept;
    static ElasticModuli2D youngs_poisson(Float E, Float nu);

    auto lambda() const noexcept { return m_lambda; }
    auto mu() const noexcept { return m_mu; }

  private:
    ElasticModuli2D() = default;
    ElasticModuli2D(Float lambda, Float mu) noexcept;
    Float m_lambda;
    Float m_mu;
};
}  // namespace uipc::constitution
```


