

# File attribute\_factory.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**attribute\_factory.h**](attribute__factory_8h.md)

[Go to the documentation of this file](attribute__factory_8h.md)


```C++
#pragma once
#include <uipc/geometry/attribute_slot.h>


namespace uipc::geometry
{
class UIPC_CORE_API AttributeFactory
{
    class Impl;

  public:
    AttributeFactory();
    ~AttributeFactory();

    [[nodiscard]] vector<S<IAttributeSlot>> from_json(const Json& j);
    [[nodiscard]] Json to_json(span<IAttribute*> attributes);

  private:
    U<Impl> m_impl;
};
}  // namespace uipc::geometry
```


