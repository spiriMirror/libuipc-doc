

# File finite\_element\_constitution.h

[**File List**](files.md) **>** [**constitution**](dir_e6404e629433dfdedefe8b8f43f6234d.md) **>** [**finite\_element\_constitution.h**](finite__element__constitution_8h.md)

[Go to the documentation of this file](finite__element__constitution_8h.md)


```C++
#pragma once
#include <uipc/constitution/constitution.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::constitution
{
class UIPC_CONSTITUTION_API FiniteElementConstitution : public IConstitution
{
    using Base = IConstitution;

  protected:
    void apply_to(geometry::SimplicialComplex& sc, Float mass_density, Float thickness = 0.0) const;
};
}  // namespace uipc::constitution
```


