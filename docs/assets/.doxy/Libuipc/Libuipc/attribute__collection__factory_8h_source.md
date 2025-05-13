

# File attribute\_collection\_factory.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**attribute\_collection\_factory.h**](attribute__collection__factory_8h.md)

[Go to the documentation of this file](attribute__collection__factory_8h.md)


```C++
#pragma once
#include <uipc/geometry/attribute_collection.h>

namespace uipc::geometry
{
class UIPC_CORE_API AttributeCollectionFactory
{
    class Impl;

  public:
    AttributeCollectionFactory();
    ~AttributeCollectionFactory();

    [[nodiscard]] S<AttributeCollection> from_json(const Json& j,
                                                   span<S<IAttributeSlot>> attributes);

    [[nodiscard]] Json to_json(const AttributeCollection* acs,
                               unordered_map<IAttribute*, IndexT> attr_to_index);

  private:
    U<Impl> m_impl;
};
}  // namespace uipc::geometry
```


