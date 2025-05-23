

# File attribute\_collection\_factory.h

[**File List**](files.md) **>** [**geometry**](dir_04894967a28d068f10a69f6e8a07a2cb.md) **>** [**attribute\_collection\_factory.h**](attribute__collection__factory_8h.md)

[Go to the documentation of this file](attribute__collection__factory_8h.md)


```C++
#pragma once
#include <uipc/geometry/attribute_collection.h>
#include <uipc/geometry/attribute_collection_commit.h>
#include <uipc/geometry/shared_attribute_context.h>

namespace uipc::geometry
{


class UIPC_CORE_API AttributeCollectionFactory
{
    class Impl;

  public:
    AttributeCollectionFactory();
    ~AttributeCollectionFactory();

    [[nodiscard]] S<AttributeCollection> from_json(const Json& j,
                                                   DeserialSharedAttributeContext& ctx);

    [[nodiscard]] Json to_json(const AttributeCollection&    ac,
                               SerialSharedAttributeContext& ctx);

    [[nodiscard]] Json commit_to_json(const AttributeCollectionCommit& acc,
                                      SerialSharedAttributeContext&    ctx);

    [[nodiscard]] S<AttributeCollectionCommit> commit_from_json(const Json& j,
                                                                DeserialSharedAttributeContext& ctx);
    [[nodiscard]] AttributeCollectionCommit diff(const AttributeCollection& current,
                                                 const AttributeCollection& reference);

  private:
    U<Impl> m_impl;
};
}  // namespace uipc::geometry
```


