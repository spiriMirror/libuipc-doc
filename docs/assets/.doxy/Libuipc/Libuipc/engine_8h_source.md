

# File engine.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**engine.h**](engine_8h.md)

[Go to the documentation of this file](engine_8h.md)


```C++
#pragma once
#include <string>
#include <uipc/common/dllexport.h>
#include <uipc/common/smart_pointer.h>
#include <uipc/core/i_engine.h>
#include <uipc/backend/visitors/world_visitor.h>
#include <uipc/common/exception.h>


namespace uipc::core
{
namespace internal
{
    class UIPC_CORE_API Engine;
}

class World;
class UIPC_CORE_API Engine final
{
  public:
    Engine(std::string_view backend_name,
           std::string_view workspace = "./",
           const Json&      config    = default_config());
    ~Engine();

    // no copy
    Engine(const Engine&)            = delete;
    Engine& operator=(const Engine&) = delete;
    // allow move
    Engine(Engine&&) noexcept            = default;
    Engine& operator=(Engine&&) noexcept = default;

    std::string_view         backend_name() const noexcept;
    std::string_view         workspace() const noexcept;
    EngineStatusCollection&  status();
    const FeatureCollection& features();
    Json                     to_json() const;
    static Json              default_config();

  private:
    friend class World;
    S<internal::Engine> m_internal;
};

class UIPC_CORE_API EngineException : public Exception
{
  public:
    using Exception::Exception;
};
}  // namespace uipc::core
```


