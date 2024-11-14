

# File sanity\_checker.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**sanity\_check**](dir_bc94a01fec317e710a764ca285cf9c79.md) **>** [**sanity\_checker.h**](sanity__checker_8h.md)

[Go to the documentation of this file](sanity__checker_8h.md)


```C++
#pragma once
#include <uipc/common/macro.h>
#include <uipc/sanity_check/i_sanity_checker.h>
#include <uipc/sanity_check/sanity_checker_auto_register.h>
#include <uipc/core/scene.h>

namespace uipc::backend
{
class SceneVisitor;
}

namespace uipc::core
{
class UIPC_CORE_API SanityChecker : public ISanityChecker
{
  public:
    explicit SanityChecker(Scene& s) noexcept;

    virtual U64               get_id() const noexcept = 0;
    virtual SanityCheckResult do_check() noexcept;

  protected:
    virtual SanityCheckResult do_check(backend::SceneVisitor& scene) noexcept = 0;

    Scene& m_scene;
};
}  // namespace uipc::core

#define REGISTER_SANITY_CHECKER(SanityChecker)                                                       \
    namespace auto_register                                                                          \
    {                                                                                                \
        static ::uipc::core::SanityCheckerAutoRegister UIPC_NAME_WITH_ID(SanityCheckerAutoRegister){ \
            ::uipc::core::detail::register_sanity_checker_creator<SanityChecker>()};                 \
    }

// End of file
```


