

# File world.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**internal**](dir_115c6c39d81d30f3e74f2509c90b0b60.md) **>** [**world.h**](internal_2world_8h.md)

[Go to the documentation of this file](internal_2world_8h.md)


```C++
#pragma once
#include <uipc/core/internal/scene.h>
#include <uipc/core/internal/engine.h>
#include <uipc/core/feature_collection.h>

namespace uipc::core::internal
{
class UIPC_CORE_API World final : public std::enable_shared_from_this<World>
{
    friend class backend::WorldVisitor;
    friend class SanityChecker;

  public:
    World(internal::Engine& e) noexcept;
    void init(internal::Scene& s);

    void advance();
    void sync();
    void retrieve();
    void backward();
    bool dump();
    bool recover(SizeT aim_frame = ~0ull);
    bool is_valid() const;

    SizeT frame() const;

    const FeatureCollection& features() const;

  private:
    internal::Scene*  m_scene  = nullptr;
    internal::Engine* m_engine = nullptr;
    bool              m_valid  = true;
    void              sanity_check(Scene& s);
};
}  // namespace uipc::core::internal
```


