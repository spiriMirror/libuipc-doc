

# File parameter\_collection.h

[**File List**](files.md) **>** [**diff\_sim**](dir_98c941875c7e3cb13f2b177552938e34.md) **>** [**parameter\_collection.h**](parameter__collection_8h.md)

[Go to the documentation of this file](parameter__collection_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/span.h>
#include <uipc/common/type_define.h>
#include <uipc/common/smart_pointer.h>
#include <uipc/common/vector.h>
#include <uipc/geometry/attribute_slot.h>
namespace uipc::core
{
class DiffSim;
}

namespace uipc::backend
{
class DiffSimVisitor;
}

namespace uipc::diff_sim
{
class Object;
class ParameterCollection;

span<Float> UIPC_CORE_API view(ParameterCollection& collection);

class UIPC_CORE_API ParameterCollection
{
  public:
    void resize(SizeT N, Float default_value = 0.0f);
    void              broadcast();
    span<const Float> view() const;

    ~ParameterCollection();

  private:
    friend class uipc::core::DiffSim;
    friend class uipc::backend::DiffSimVisitor;

    ParameterCollection();

    // delete copy constructor and assignment operator
    ParameterCollection(const ParameterCollection&)            = delete;
    ParameterCollection& operator=(const ParameterCollection&) = delete;

    class Impl;
    friend span<Float> UIPC_CORE_API view(ParameterCollection& collection);
    void connect(S<geometry::IAttributeSlot> diff_parm_slot,
                 S<geometry::IAttributeSlot> parm_slot);
    void build();

    bool    need_backend_broadcast() const;
    void    need_backend_broadcast(bool v);
    U<Impl> m_impl;
};
}  // namespace uipc::diff_sim
```


