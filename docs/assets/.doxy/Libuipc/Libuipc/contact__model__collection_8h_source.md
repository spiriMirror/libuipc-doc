

# File contact\_model\_collection.h

[**File List**](files.md) **>** [**core**](dir_eca9d1283f7cad9ff89c5ab44937d4d9.md) **>** [**contact\_model\_collection.h**](contact__model__collection_8h.md)

[Go to the documentation of this file](contact__model__collection_8h.md)


```C++
#pragma once
#include <uipc/geometry/attribute_collection.h>

namespace uipc::geometry
{
template <typename T>
class AttributeFriend;
}

namespace uipc::core
{
class ContactTabular;

template <bool IsConst>
class ContactModelCollectionT
{
    template <typename T>
    friend class geometry::AttributeFriend;

    friend class ContactTabular;
    using AutoAttributeCollection =
        std::conditional_t<IsConst, const geometry::AttributeCollection, geometry::AttributeCollection>;

    // Only called by ContactTabular
    ContactModelCollectionT(AutoAttributeCollection& attributes)
        : m_attributes(attributes)
    {
    }

  public:
    template <typename T>
    auto create(std::string_view name, const T& default_value = {}, bool allow_destroy = true)
        requires(!IsConst)
    {
        return m_attributes.template create<T>(name, default_value, allow_destroy);
    }

    template <typename T>
    auto find(std::string_view name)
    {
        return m_attributes.template find<T>(name);
    }

    auto find(std::string_view name) { return m_attributes.find(name); }

    auto to_json() const { return m_attributes.to_json(); }

  private:
    AutoAttributeCollection& m_attributes;
};

using ContactModelCollection  = ContactModelCollectionT<false>;
using CContactModelCollection = ContactModelCollectionT<true>;
}  // namespace uipc::core
```


