

# File diff\_sim.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**diff\_sim.h**](diff__sim_8h.md)

[Go to the documentation of this file](diff__sim_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/diff_sim/parameter_collection.h>
#include <uipc/diff_sim/sparse_coo_view.h>

namespace uipc::backend
{
class SceneVisitor;
class DiffSimVisitor;
}  // namespace uipc::backend

namespace uipc::core::internal
{
class Scene;
}

namespace uipc::core
{
class Scene;
class UIPC_CORE_API DiffSim
{
    friend class Scene;
    friend class internal::Scene;
    friend class backend::DiffSimVisitor;


    DiffSim();

    // delete copy constructor and assignment operator
    DiffSim(const DiffSim&)            = delete;
    DiffSim& operator=(const DiffSim&) = delete;

  public:
    diff_sim::ParameterCollection&       parameters();
    const diff_sim::ParameterCollection& parameters() const;
    ~DiffSim();

  private:
    class Impl;
    U<Impl> m_impl;

    void init(internal::Scene& scene);  // only be called by Scene
};
}  // namespace uipc::core
```


