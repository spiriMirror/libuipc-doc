

# File platform\_handle.h

[**File List**](files.md) **>** [**common**](dir_a4796c188772d0a0fa09f1942d616969.md) **>** [**platform\_handle.h**](platform__handle_8h.md)

[Go to the documentation of this file](platform__handle_8h.md)


```C++
#pragma once
#include <GLFW/glfw3.h>
#include <bgfx/bgfx.h>
namespace uipc::gui
{
void* glfw_native_window_handle(GLFWwindow* window);

bgfx::NativeWindowHandleType::Enum native_window_handle_type();

void* native_display_handle();
}
```


