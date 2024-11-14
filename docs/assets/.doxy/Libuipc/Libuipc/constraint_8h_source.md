

# File constraint.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**constraint.h**](constraint_8h.md)

[Go to the documentation of this file](constraint_8h.md)


```C++
#pragma once
#include <uipc/constitution/constitution.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::constitution
{
class UIPC_CORE_API Constraint : public IConstitution
{
  public:
    Constraint() noexcept;

  protected:
    virtual U64 get_uid() const noexcept = 0;

    void apply_to(geometry::SimplicialComplex& sc) const;
};
}  // namespace uipc::constitution
```


