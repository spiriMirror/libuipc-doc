

# File resident\_thread.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**resident\_thread.h**](resident__thread_8h.md)

[Go to the documentation of this file](resident__thread_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/common/smart_pointer.h>

namespace uipc
{
class UIPC_CORE_API ResidentThread
{
  public:
    ResidentThread();

    SizeT hash() const;

    ~ResidentThread();

    bool post(std::function<void()> task);
    bool is_ready() const;

    class Impl;

  private:
    S<Impl> m_impl;
};
}  // namespace uipc
```


