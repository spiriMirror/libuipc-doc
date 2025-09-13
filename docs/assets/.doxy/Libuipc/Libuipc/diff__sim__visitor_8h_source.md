

# File diff\_sim\_visitor.h

[**File List**](files.md) **>** [**backend**](dir_53d62147b82bd29328805b2087bd1012.md) **>** [**visitors**](dir_007753111df00039ee3ec058cc286377.md) **>** [**diff\_sim\_visitor.h**](diff__sim__visitor_8h.md)

[Go to the documentation of this file](diff__sim__visitor_8h.md)


```C++
#pragma once
#include <uipc/diff_sim/parameter_collection.h>
#include <uipc/diff_sim/sparse_coo_view.h>

namespace uipc::core
{
class DiffSim;
}
namespace uipc::backend
{
class UIPC_CORE_API DiffSimVisitor
{
  public:
    DiffSimVisitor(core::DiffSim& diff_sim);
    ~DiffSimVisitor();
    diff_sim::ParameterCollection&       parameters();
    const diff_sim::ParameterCollection& parameters() const;

  private:
    core::DiffSim& m_diff_sim;
};
}  // namespace uipc::backend
```


