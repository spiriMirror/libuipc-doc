

# File macro.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**macro.h**](common_2macro_8h.md)

[Go to the documentation of this file](common_2macro_8h.md)


```C++
#pragma once

#define UIPC_TO_STRING(x) #x

#define UIPC_CONCATE(x, y) x##y

// indirection to allow the __COUNTER__ macro to be expanded
#define UIPC_NAME_WITH_ID_IMPL(x, ID) UIPC_CONCATE(x, ID)

// create a unique name with the __COUNTER__ macro appended
#define UIPC_NAME_WITH_ID(x) UIPC_NAME_WITH_ID_IMPL(x, __COUNTER__)
```


