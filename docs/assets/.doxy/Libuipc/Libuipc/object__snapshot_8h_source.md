

# File object\_snapshot.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**object\_snapshot.h**](object__snapshot_8h.md)

[Go to the documentation of this file](object__snapshot_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/type_define.h>
#include <uipc/common/vector.h>
#include <uipc/common/json.h>

namespace uipc::core::internal
{
class Scene;
}
namespace uipc::core
{
class SceneFactory;

class SceneSnapshot;

class Object;

class UIPC_CORE_API ObjectSnapshot
{
    friend class SceneSnapshot;
    friend class SceneFactory;
    friend class ObjectCollection;
    friend class internal::Scene;
    friend class Object;

    friend UIPC_CORE_API void to_json(Json& j, const ObjectSnapshot& snapshot);
    friend UIPC_CORE_API void from_json(const Json& j, ObjectSnapshot& snapshot);

  public:
    ObjectSnapshot() = default;
    ObjectSnapshot(const Object& object);
    IndexT id() const noexcept { return m_id; }

  private:
    IndexT         m_id;
    std::string    m_name;
    vector<IndexT> m_geometries;
};

UIPC_CORE_API void to_json(Json& j, const ObjectSnapshot& snapshot);
UIPC_CORE_API void from_json(const Json& j, ObjectSnapshot& snapshot);
}  // namespace uipc::core
```


