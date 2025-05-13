

# File scene\_factory.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**scene\_factory.h**](scene__factory_8h.md)

[Go to the documentation of this file](scene__factory_8h.md)


```C++
#pragma once
#include <uipc/core/scene.h>

namespace uipc::core
{
class UIPC_CORE_API SceneFactory
{
    class Impl;

  public:
    SceneFactory();
    ~SceneFactory();

    [[nodiscard]] S<Scene> from_json(const Json& j);
    [[nodiscard]] Json     to_json(const Scene& scene);

  private:
    U<Impl> m_impl;
};
}  // namespace uipc::core
```


