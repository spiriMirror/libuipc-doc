

# File constitution.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**constitution.h**](constitution_8h.md)

[Go to the documentation of this file](constitution_8h.md)


```C++
#pragma once
#include <string_view>
#include <uipc/geometry/geometry.h>
#include <uipc/builtin/constitution_uid_collection.h>

namespace uipc::constitution
{
class UIPC_CORE_API IConstitution
{
  public:
    virtual ~IConstitution() = default;
    U64                     uid() const noexcept;
    std::string_view        name() const noexcept;
    std::string_view        type() const noexcept;
    const builtin::UIDInfo& uid_info() const noexcept;


  protected:
    virtual U64 get_uid() const noexcept = 0;
};
}  // namespace uipc::constitution
```


