

# File adjoint\_method\_feature.h

[**File List**](files.md) **>** [**diff\_sim**](dir_98c941875c7e3cb13f2b177552938e34.md) **>** [**adjoint\_method\_feature.h**](adjoint__method__feature_8h.md)

[Go to the documentation of this file](adjoint__method__feature_8h.md)


```C++
#pragma 
#include <uipc/core/feature.h>
#include <uipc/backend/buffer_view.h>

namespace uipc::diff_sim
{
class UIPC_CORE_API AdjointMethodFeatureOverrider
{
  public:
    virtual void do_select_dofs(SizeT frame, backend::BufferView in_SDI) = 0;
    virtual void do_receive_dofs(backend::BufferView out_dofs)           = 0;
    virtual void do_compute_dLdP(backend::BufferView out_dLdP,
                                 backend::BufferView in_dLdx)            = 0;
};

class UIPC_CORE_API AdjointMethodFeature final : public core::Feature
{
    class Impl;

  public:
    constexpr static std::string_view FeatureName = "diff_sim/adjoint_method";

    AdjointMethodFeature(S<AdjointMethodFeatureOverrider> overrider);

    void select_dofs(SizeT frame, backend::BufferView in_SDI);

    void receive_dofs(backend::BufferView out_Dofs);

    void compute_dLdP(backend::BufferView out_dLdP, backend::BufferView in_dLdX);

  private:
    virtual std::string_view         get_name() const final override;
    S<AdjointMethodFeatureOverrider> m_impl;
    SizeT                            last_calling_frame = 0;
};
}  // namespace uipc::diff_sim
```


