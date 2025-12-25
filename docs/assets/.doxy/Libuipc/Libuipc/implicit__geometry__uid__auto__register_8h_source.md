

# File implicit\_geometry\_uid\_auto\_register.h

[**File List**](files.md) **>** [**builtin**](dir_e46c520626162f9e42d80fd08f196511.md) **>** [**implicit\_geometry\_uid\_auto\_register.h**](implicit__geometry__uid__auto__register_8h.md)

[Go to the documentation of this file](implicit__geometry__uid__auto__register_8h.md)


```C++
#pragma once
#include <uipc/builtin/uid_register.h>
#include <uipc/common/list.h>

namespace uipc::builtin
{
class UIPC_CORE_API ImplicitGeometryUIDAutoRegister
{
  public:
    using Creator = UIDInfoCreator;

    ImplicitGeometryUIDAutoRegister(Creator creator) noexcept;

  private:
    friend class ImplicitGeometryUIDCollection;
    static list<Creator>& creators() noexcept;
};
}  // namespace uipc::builtin

#define REGISTER_IMPLICIT_GEOMETRY_UIDS_INTERNAL(counter)                                                 \
    namespace auto_register                                                                               \
    {                                                                                                     \
        static ::uipc::list<::uipc::builtin::UIDInfo> ImplicitGeometryUIDAutoRegisterFunction##counter(); \
        static ::uipc::builtin::ImplicitGeometryUIDAutoRegister ImplicitGeometryUIDAutoRegister##counter{ \
            ::uipc::builtin::ImplicitGeometryUIDAutoRegister::Creator{                                    \
                ImplicitGeometryUIDAutoRegisterFunction##counter, __FILE__, __LINE__}};                   \
    }                                                                                                     \
    static ::uipc::list<::uipc::builtin::UIDInfo> auto_register::ImplicitGeometryUIDAutoRegisterFunction##counter()

#define REGISTER_IMPLICIT_GEOMETRY_UIDS(...) REGISTER_IMPLICIT_GEOMETRY_UIDS_INTERNAL(__COUNTER__)
```


