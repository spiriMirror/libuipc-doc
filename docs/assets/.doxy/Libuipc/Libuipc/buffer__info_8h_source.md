

# File buffer\_info.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**buffer\_info.h**](buffer__info_8h.md)

[Go to the documentation of this file](buffer__info_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/common/vector.h>
namespace uipc
{
class BufferInfo
{
  public:
    void*         data;
    size_t        itemsize;
    vector<int64_t> shape;
    vector<int64_t> strides;
};
}  // namespace uipc
```


