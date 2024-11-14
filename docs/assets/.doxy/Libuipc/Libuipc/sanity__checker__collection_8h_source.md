

# File sanity\_checker\_collection.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**sanity\_check**](dir_bc94a01fec317e710a764ca285cf9c79.md) **>** [**sanity\_checker\_collection.h**](sanity__checker__collection_8h.md)

[Go to the documentation of this file](sanity__checker__collection_8h.md)


```C++
#pragma once
#include <uipc/common/smart_pointer.h>
#include <uipc/common/list.h>
#include <uipc/sanity_check/i_sanity_checker.h>

namespace uipc::core
{
class Scene;
class SanityCheckerCollection
{
  public:
    SanityCheckerCollection() noexcept = default;
    void              init(Scene& s);
    SanityCheckResult check() const;

  private:
    list<U<ISanityChecker>> entries;
};
}  // namespace uipc::core
```


