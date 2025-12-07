

# File world.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**world.h**](world_8h.md)

[Go to the documentation of this file](world_8h.md)


```C++
#pragma once
#include <uipc/core/sanity_checker.h>
#include <uipc/core/scene.h>
#include <uipc/core/feature_collection.h>

namespace uipc::backend
{
class WorldVisitor;
}

namespace uipc::core::internal
{
class World;
}

namespace uipc::core
{
class Engine;

class UIPC_CORE_API World final
{
    friend class backend::WorldVisitor;
    friend class SanityChecker;

  public:
    World(Engine& e) noexcept;
    ~World();

    World(const World&)            = delete;
    World(World&&)                 = default;
    World& operator=(const World&) = delete;
    World& operator=(World&&)      = default;

    void init(Scene& s);

    void advance();
    void sync();
    void retrieve();
    bool dump();
    bool recover(SizeT aim_frame = ~0ull);
    bool is_valid() const;

    SizeT frame() const;

    const FeatureCollection& features() const;
    SanityChecker&           sanity_checker();
    const SanityChecker&     sanity_checker() const;

    // Allow create a core::World from a core::internal::World
    World(S<internal::World> w) noexcept;

  private:
    S<internal::World> m_internal;
};
}  // namespace uipc::core
```


