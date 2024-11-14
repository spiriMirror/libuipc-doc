

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
class World;
class UIPC_CORE_API Engine final
{
    class Impl;

  public:
    Engine(std::string_view backend_name,
           std::string_view workspace = "./",
           const Json&      config    = default_config());
    ~Engine();

    std::string_view        backend_name() const noexcept;
    std::string_view        workspace() const noexcept;
    EngineStatusCollection& status();

    Json to_json() const;

    static Json default_config();

  private:
    friend class World;

    void  init(backend::WorldVisitor v);  // only be called by World
    void  advance();                      // only be called by World
    void  backward();                     // only be called by World
    void  sync();                         // only be called by World
    void  retrieve();                     // only be called by World
    bool  dump();                         // only be called by World
    bool  recover(SizeT dst_frame);       // only be called by World
    SizeT frame() const;                  // only be called by World

    U<Impl> m_impl;
};

class UIPC_CORE_API EngineException : public Exception
{
  public:
    using Exception::Exception;
};
}  // namespace uipc::core
```


