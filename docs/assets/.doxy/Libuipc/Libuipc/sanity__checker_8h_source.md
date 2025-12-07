

# File sanity\_checker.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**sanity\_checker.h**](sanity__checker_8h.md)

[Go to the documentation of this file](sanity__checker_8h.md)


```C++
#pragma once
#include <uipc/core/i_sanity_checker.h>

namespace uipc::core::internal
{
class Scene;
}

namespace uipc::core
{
class Scene;

class UIPC_CORE_API SanityChecker final
{
  public:
    SanityChecker(internal::Scene& scene, std::string_view workspace);
    ~SanityChecker();

    SanityCheckResult check();
    void              report();

    const unordered_map<U64, S<SanityCheckMessage>>& errors() const;
    const unordered_map<U64, S<SanityCheckMessage>>& warns() const;
    const unordered_map<U64, S<SanityCheckMessage>>& infos() const;

    void clear();

  private:
    core::SanityCheckMessageCollection m_errors;
    core::SanityCheckMessageCollection m_warns;
    core::SanityCheckMessageCollection m_infos;

    internal::Scene& m_scene;
    std::string      m_workspace;
};
}  // namespace uipc::core
```


