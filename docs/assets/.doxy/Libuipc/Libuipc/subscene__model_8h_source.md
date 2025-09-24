

# File subscene\_model.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**subscene\_model.h**](subscene__model_8h.md)

[Go to the documentation of this file](subscene__model_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/type_define.h>
#include <uipc/common/json.h>

namespace uipc::core
{
class UIPC_CORE_API SubsceneModel
{
  public:
    SubsceneModel() noexcept;
    SubsceneModel(const Vector2i& ids, bool enable, const Json& config);

    const Vector2i& topo() const;
    bool            is_enabled() const;
    const Json&     config() const;

    friend void to_json(Json& json, const SubsceneModel& model);
    friend void from_json(const Json& json, SubsceneModel& model);

  private:
    Vector2i m_ids;
    bool     m_is_enabled;
    Json     m_config;
};

void to_json(Json& json, const SubsceneModel& model);

void from_json(const Json& json, SubsceneModel& model);
}  // namespace uipc::core
```


