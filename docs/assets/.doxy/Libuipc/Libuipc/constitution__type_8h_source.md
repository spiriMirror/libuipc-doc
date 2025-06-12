

# File constitution\_type.h

[**File List**](files.md) **>** [**builtin**](dir_e46c520626162f9e42d80fd08f196511.md) **>** [**constitution\_type.h**](constitution__type_8h.md)

[Go to the documentation of this file](constitution__type_8h.md)


```C++
#pragma once
#include <string_view>

namespace uipc::builtin
{
constexpr std::string_view AffineBody      = "AffineBody";
constexpr std::string_view InterAffineBody = "InterAffineBody";
constexpr std::string_view FiniteElement   = "FiniteElement";
constexpr std::string_view Constraint      = "Constraint";
}  // namespace uipc::builtin
```


