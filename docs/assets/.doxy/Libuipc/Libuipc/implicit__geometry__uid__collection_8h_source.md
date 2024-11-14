

# File implicit\_geometry\_uid\_collection.h

[**File List**](files.md) **>** [**builtin**](dir_e46c520626162f9e42d80fd08f196511.md) **>** [**implicit\_geometry\_uid\_collection.h**](implicit__geometry__uid__collection_8h.md)

[Go to the documentation of this file](implicit__geometry__uid__collection_8h.md)


```C++
#pragma once
#include <uipc/builtin/uid_register.h>


namespace uipc::builtin
{
class UIPC_CORE_API ImplicitGeometryUIDCollection : public details::UIDRegister
{
  public:
    static const ImplicitGeometryUIDCollection& instance() noexcept;

  private:
    ImplicitGeometryUIDCollection();
};
}  // namespace uipc::builtin
```


