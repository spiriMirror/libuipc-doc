

# File const\_string\_map.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**const\_string\_map.h**](const__string__map_8h.md)

[Go to the documentation of this file](const__string__map_8h.md)


```C++
#pragma once
#include <string>
#include <string_view>
#include <uipc/common/unordered_set.h>

namespace uipc
{
class ConstStringMap
{
  public:
    std::string_view operator[](std::string_view content);

  private:
    std::unordered_set<std::string> m_pool;
    std::mutex                      m_mutex;
};
}  // namespace uipc
```


