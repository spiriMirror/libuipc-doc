

# File stack.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**stack.h**](stack_8h.md)

[Go to the documentation of this file](stack_8h.md)


```C++
#pragma once
#include <stack>
#include <deque>

namespace uipc
{
template <typename T>
using stack = std::stack<T, std::pmr::deque<T>>;
}
```


