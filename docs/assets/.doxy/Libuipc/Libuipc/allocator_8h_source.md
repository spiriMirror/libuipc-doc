

# File allocator.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**allocator.h**](allocator_8h.md)

[Go to the documentation of this file](allocator_8h.md)


```C++
#pragma once
#include <memory_resource>

namespace uipc
{
template <typename T>
using Allocator = std::pmr::polymorphic_allocator<T>;
}
```


