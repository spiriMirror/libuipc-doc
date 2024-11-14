

# File animator\_visitor.h

[**File List**](files.md) **>** [**backend**](dir_53d62147b82bd29328805b2087bd1012.md) **>** [**visitors**](dir_007753111df00039ee3ec058cc286377.md) **>** [**animator\_visitor.h**](animator__visitor_8h.md)

[Go to the documentation of this file](animator__visitor_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/common/dllexport.h>

namespace uipc::core
{
class Animator;
}

namespace uipc::backend
{
class UIPC_CORE_API AnimatorVisitor
{
  public:
    AnimatorVisitor(core::Animator& animator) noexcept;
    void  init();
    void  update();
    SizeT substep() noexcept;

  private:
    core::Animator& m_animator;
};
}  // namespace uipc::backend
```


