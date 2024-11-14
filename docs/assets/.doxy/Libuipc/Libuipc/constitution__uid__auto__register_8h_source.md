

# File constitution\_uid\_auto\_register.h

[**File List**](files.md) **>** [**builtin**](dir_e46c520626162f9e42d80fd08f196511.md) **>** [**constitution\_uid\_auto\_register.h**](constitution__uid__auto__register_8h.md)

[Go to the documentation of this file](constitution__uid__auto__register_8h.md)


```C++
#pragma once
#include <uipc/builtin/uid_register.h>
#include <uipc/common/list.h>

namespace uipc::builtin
{
class UIPC_CORE_API ConstitutionUIDAutoRegister
{
  public:
    using Creator = std::function<list<UIDInfo>()>;
    ConstitutionUIDAutoRegister(Creator creator) noexcept;

  private:
    friend class ConstitutionUIDCollection;
    static list<Creator>& creators() noexcept;
};
}  // namespace uipc::builtin

#define REGISTER_CONSTITUTION_UIDS_INTERNAL(counter)                                                  \
    namespace auto_register                                                                           \
    {                                                                                                 \
        static ::uipc::list<::uipc::builtin::UIDInfo> ConstitutionUIDAutoRegisterFunction##counter(); \
        static ::uipc::builtin::ConstitutionUIDAutoRegister ConstitutionUIDAutoRegister##counter{     \
            ConstitutionUIDAutoRegisterFunction##counter};                                            \
    }                                                                                                 \
    static ::uipc::list<::uipc::builtin::UIDInfo> auto_register::ConstitutionUIDAutoRegisterFunction##counter()

#define REGISTER_CONSTITUTION_UIDS(...)                                        \
    REGISTER_CONSTITUTION_UIDS_INTERNAL(__COUNTER__)
```


