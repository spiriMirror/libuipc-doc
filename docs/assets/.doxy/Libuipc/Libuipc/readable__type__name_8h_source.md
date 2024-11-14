

# File readable\_type\_name.h

[**File List**](files.md) **>** [**common**](dir_fe04c8fb910be76d82cd33e795163b9b.md) **>** [**readable\_type\_name.h**](readable__type__name_8h.md)

[Go to the documentation of this file](readable__type__name_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <string_view>
#include <boost/core/demangle.hpp>
#define READABLE_TYPE_NAME_AS_ALIAS(type)                                      \
    template <>                                                                \
    inline std::string readable_type_name<type>() noexcept                     \
    {                                                                          \
        return #type;                                                          \
    }

namespace uipc
{
template <typename T>
inline std::string readable_type_name() noexcept
{
    return boost::core::demangle(typeid(T).name());
}

READABLE_TYPE_NAME_AS_ALIAS(Vector2);
READABLE_TYPE_NAME_AS_ALIAS(Vector3);
READABLE_TYPE_NAME_AS_ALIAS(Vector4);

READABLE_TYPE_NAME_AS_ALIAS(Vector2i);
READABLE_TYPE_NAME_AS_ALIAS(Vector3i);
READABLE_TYPE_NAME_AS_ALIAS(Vector4i);

READABLE_TYPE_NAME_AS_ALIAS(Vector6);
READABLE_TYPE_NAME_AS_ALIAS(Vector9);
READABLE_TYPE_NAME_AS_ALIAS(Vector12);

READABLE_TYPE_NAME_AS_ALIAS(Matrix2x2);
READABLE_TYPE_NAME_AS_ALIAS(Matrix3x3);
READABLE_TYPE_NAME_AS_ALIAS(Matrix4x4);

READABLE_TYPE_NAME_AS_ALIAS(Matrix6x6);
READABLE_TYPE_NAME_AS_ALIAS(Matrix9x9);
READABLE_TYPE_NAME_AS_ALIAS(Matrix12x12);

READABLE_TYPE_NAME_AS_ALIAS(VectorX);
READABLE_TYPE_NAME_AS_ALIAS(VectorXi);
READABLE_TYPE_NAME_AS_ALIAS(VectorXi64);
READABLE_TYPE_NAME_AS_ALIAS(VectorXu);
READABLE_TYPE_NAME_AS_ALIAS(VectorXu64);
}  // namespace uipc

#undef READABLE_TYPE_NAME_AS_ALIAS
```

