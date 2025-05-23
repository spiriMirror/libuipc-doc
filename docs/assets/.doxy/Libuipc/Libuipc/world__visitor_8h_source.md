

# File world\_visitor.h

[**File List**](files.md) **>** [**backend**](dir_53d62147b82bd29328805b2087bd1012.md) **>** [**visitors**](dir_007753111df00039ee3ec058cc286377.md) **>** [**world\_visitor.h**](world__visitor_8h.md)

[Go to the documentation of this file](world__visitor_8h.md)


```C++
#pragma once
#include <uipc/backend/visitors/scene_visitor.h>
#include <uipc/backend/visitors/animator_visitor.h>
namespace uipc::core
{
class World;
class Engine;
}  // namespace uipc::core

namespace uipc::core::internal
{
class World;
class Scene;
class Engine;
}  // namespace uipc::core::internal

namespace uipc::backend
{
class UIPC_CORE_API WorldVisitor
{
  public:
    WorldVisitor(core::World& w) noexcept;
    WorldVisitor(core::internal::World& w) noexcept;

    WorldVisitor(const WorldVisitor&)            = delete;
    WorldVisitor(WorldVisitor&&)                 = default;
    WorldVisitor& operator=(const WorldVisitor&) = delete;
    WorldVisitor& operator=(WorldVisitor&&)      = default;

    SceneVisitor    scene() noexcept;
    AnimatorVisitor animator() noexcept;
    core::World&    ref() noexcept;

  private:
    mutable S<core::World> m_ref;
    core::internal::World& m_world;
};
}  // namespace uipc::backend
```


