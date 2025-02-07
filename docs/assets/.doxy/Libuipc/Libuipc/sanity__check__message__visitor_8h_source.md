

# File sanity\_check\_message\_visitor.h

[**File List**](files.md) **>** [**backend**](dir_53d62147b82bd29328805b2087bd1012.md) **>** [**visitors**](dir_007753111df00039ee3ec058cc286377.md) **>** [**sanity\_check\_message\_visitor.h**](sanity__check__message__visitor_8h.md)

[Go to the documentation of this file](sanity__check__message__visitor_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/core/i_sanity_checker.h>

namespace uipc::backend
{
class UIPC_CORE_API SanityCheckMessageVisitor
{
  public:
    SanityCheckMessageVisitor(core::SanityCheckMessage& msg) noexcept;

    auto& id() const noexcept { return m_msg.m_id; }
    auto& name() const noexcept { return m_msg.m_name; }
    auto& result() const noexcept { return m_msg.m_result; }
    auto& message() const noexcept { return m_msg.m_message; }
    auto& geometries() const noexcept { return m_msg.m_geometries; }

  private:
    core::SanityCheckMessage& m_msg;
};
}  // namespace uipc::backend
```


