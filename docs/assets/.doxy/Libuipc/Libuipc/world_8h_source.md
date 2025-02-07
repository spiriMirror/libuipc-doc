

# File world.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**world.h**](world_8h.md)

[Go to the documentation of this file](world_8h.md)


```C++
#pragma once
#include <uipc/core/scene.h>

namespace uipc::backend
{
class WorldVisitor;
}

namespace uipc::core
{
class Engine;
}

namespace uipc::core
{
class UIPC_CORE_API World final
{
    friend class backend::WorldVisitor;
    friend class SanityChecker;

  public:
    World(Engine& e) noexcept;
    void init(Scene& s);

    void advance();
    void sync();
    void retrieve();
    void backward();
    bool dump();
    bool recover(SizeT aim_frame = ~0ull);
    bool is_valid() const;

    SizeT frame() const;

  private:
    Scene*        m_scene  = nullptr;
    core::Engine* m_engine = nullptr;
    bool          m_valid  = true;
    void          sanity_check(Scene& s);
};
}  // namespace uipc::core
```


