

# File enable\_grad\_feature.h

[**File List**](files.md) **>** [**diff\_sim**](dir_98c941875c7e3cb13f2b177552938e34.md) **>** [**enable\_grad\_feature.h**](enable__grad__feature_8h.md)

[Go to the documentation of this file](enable__grad__feature_8h.md)


```C++
#pragma once
#include <uipc/core/feature.h>
#include <uipc/common/smart_pointer.h>

namespace uipc::diff_sim
{
class UIPC_CORE_API EnableGradFeatureOverrider
{
  public:
    virtual void do_no_grad()                = 0;
    virtual void do_with_grad()              = 0;
    virtual bool get_is_grad_enabled() const = 0;
};

class UIPC_CORE_API EnableGradFeature final : public core::Feature
{
  public:
    static constexpr std::string_view FeatureName = "diff_sim/enable_grad";

    EnableGradFeature(S<EnableGradFeatureOverrider> overrider);

    void no_grad();

    void with_grad();

    bool is_grad_enabled() const;

  private:
    virtual std::string_view      get_name() const override final;
    S<EnableGradFeatureOverrider> m_impl;
};
}  // namespace uipc::diff_sim
```


