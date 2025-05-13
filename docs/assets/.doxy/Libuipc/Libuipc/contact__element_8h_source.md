

# File contact\_element.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**contact\_element.h**](contact__element_8h.md)

[Go to the documentation of this file](contact__element_8h.md)


```C++
#pragma once
#include <uipc/common/type_define.h>
#include <uipc/common/string.h>
#include <uipc/common/json.h>
#include <uipc/geometry/geometry.h>
namespace uipc::core
{
class UIPC_CORE_API ContactElement
{
  public:
    ContactElement() = default;

    ContactElement(const ContactElement&)            = default;
    ContactElement(ContactElement&&)                 = default;
    ContactElement& operator=(const ContactElement&) = default;
    ContactElement& operator=(ContactElement&&)      = default;

    ContactElement(IndexT id, std::string_view name) noexcept;
    IndexT           id() const noexcept;
    std::string_view name() const noexcept;

    friend void to_json(Json& j, const ContactElement& element);
    friend void from_json(const Json& j, ContactElement& element);

    S<geometry::AttributeSlot<IndexT>> apply_to(geometry::Geometry& geo) const;

  private:
    IndexT m_id = -1;
    string m_name;
};

void to_json(Json& j, const ContactElement& element);
void from_json(const Json& j, ContactElement& element);

}  // namespace uipc::core
```


