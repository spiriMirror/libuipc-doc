

# File constitution\_uid\_collection.h

[**File List**](files.md) **>** [**builtin**](dir_e46c520626162f9e42d80fd08f196511.md) **>** [**constitution\_uid\_collection.h**](constitution__uid__collection_8h.md)

[Go to the documentation of this file](constitution__uid__collection_8h.md)


```C++
#pragma once
#include <uipc/builtin/uid_register.h>

namespace uipc::builtin
{
class UIPC_CORE_API ConstitutionUIDCollection : public details::UIDRegister
{
  public:
    static const ConstitutionUIDCollection& instance() noexcept;

  private:
    ConstitutionUIDCollection();
};
}  // namespace uipc::builtin
```


