

# File exception.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**exception.h**](exception_8h.md)

[Go to the documentation of this file](exception_8h.md)


```C++
#pragma once
#include <uipc/common/string.h>
#include <uipc/common/dllexport.h>
#include <exception>

namespace uipc
{
class UIPC_CORE_API Exception : public std::exception
{
  public:
    Exception(const string& msg);

    virtual const char* what() const noexcept override;

  private:
    string m_msg;
};
}  // namespace uipc
```


