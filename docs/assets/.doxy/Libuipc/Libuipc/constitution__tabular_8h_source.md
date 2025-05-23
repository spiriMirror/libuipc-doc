

# File constitution\_tabular.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**constitution\_tabular.h**](constitution__tabular_8h.md)

[Go to the documentation of this file](constitution__tabular_8h.md)


```C++
#pragma once
#include <uipc/constitution/constitution.h>
#include <uipc/builtin/constitution_type.h>
#include <uipc/common/span.h>
#include <uipc/common/set.h>

namespace uipc::backend
{
class SceneVisitor;
}

namespace uipc::core::internal
{
class Scene;
}

namespace uipc::core
{
class UIPC_CORE_API ConstitutionTabular
{
    friend class internal::Scene;

  public:
    ConstitutionTabular() noexcept;
    ~ConstitutionTabular() noexcept;
    // delete copy
    ConstitutionTabular(const ConstitutionTabular&)            = delete;
    ConstitutionTabular& operator=(const ConstitutionTabular&) = delete;

    void      insert(const constitution::IConstitution& constitution);
    span<U64> uids() const noexcept;
    const set<std::string>& types() const noexcept;

  private:
    class Impl;
    U<Impl> m_impl;
    friend class Scene;
    void init(internal::Scene& scene);  // only be called by Scene.
};
}  // namespace uipc::core
```


