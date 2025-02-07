

# File contact\_tabular\_visitor.h

[**File List**](files.md) **>** [**backend**](dir_53d62147b82bd29328805b2087bd1012.md) **>** [**visitors**](dir_007753111df00039ee3ec058cc286377.md) **>** [**contact\_tabular\_visitor.h**](contact__tabular__visitor_8h.md)

[Go to the documentation of this file](contact__tabular__visitor_8h.md)


```C++
#pragma once
#include <uipc/geometry/attribute_collection.h>

namespace uipc::core
{
class ContactTabular;
}

namespace uipc::backend
{
class UIPC_CORE_API ContactTabularVisitor
{
  public:
    ContactTabularVisitor(core::ContactTabular& contact_tabular) noexcept
        : m_contact_tabular(contact_tabular)
    {
    }

    geometry::AttributeCollection& contact_models() noexcept;

  private:
    core::ContactTabular& m_contact_tabular;
};
}  // namespace uipc::backend
```


