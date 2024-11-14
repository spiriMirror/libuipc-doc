

# File sanity\_checker\_auto\_register.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**sanity\_check**](dir_bc94a01fec317e710a764ca285cf9c79.md) **>** [**sanity\_checker\_auto\_register.h**](sanity__checker__auto__register_8h.md)

[Go to the documentation of this file](sanity__checker__auto__register_8h.md)


```C++
#pragma once
#include <functional>
#include <uipc/common/smart_pointer.h>
#include <uipc/common/list.h>
#include <uipc/common/type_traits.h>
#include <uipc/sanity_check/i_sanity_checker.h>
namespace uipc::core
{
class UIPC_CORE_API SanityCheckerAutoRegister
{
    friend class Scene;
    friend class SanityCheckerCollection;

  public:
    using Creator = std::function<U<ISanityChecker>(Scene&)>;

    SanityCheckerAutoRegister(Creator&& reg);

    class Creators
    {
      public:
        list<Creator> entries;
    };

  private:
    static Creators& creators();
};

namespace detail
{
    template <std::derived_from<ISanityChecker> SanityCheckerT>
    SanityCheckerAutoRegister::Creator register_sanity_checker_creator()
    {
        return [](Scene& scene) -> U<ISanityChecker>
        {
            return ::uipc::static_pointer_cast<ISanityChecker>(
                ::uipc::make_unique<SanityCheckerT>(scene));
        };
    }
}  // namespace detail
}  // namespace uipc::core
```


