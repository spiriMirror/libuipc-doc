

# File subscene\_tabular\_visitor.h

[**File List**](files.md) **>** [**backend**](dir_53d62147b82bd29328805b2087bd1012.md) **>** [**visitors**](dir_007753111df00039ee3ec058cc286377.md) **>** [**subscene\_tabular\_visitor.h**](subscene__tabular__visitor_8h.md)

[Go to the documentation of this file](subscene__tabular__visitor_8h.md)


```C++
#pragma once
#include <uipc/geometry/attribute_collection.h>

namespace uipc::core
{
class SubsceneTabular;
}

namespace uipc::backend
{
class UIPC_CORE_API SubsceneTabularVisitor
{
  public:
    SubsceneTabularVisitor(core::SubsceneTabular& subscene_tabular) noexcept
        : m_subscene_tabular(subscene_tabular)
    {
    }

    geometry::AttributeCollection& subscene_models() noexcept;

  private:
    core::SubsceneTabular& m_subscene_tabular;
};
}  // namespace uipc::backend
```


