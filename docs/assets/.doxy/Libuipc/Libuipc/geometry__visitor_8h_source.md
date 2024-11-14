

# File geometry\_visitor.h

[**File List**](files.md) **>** [**backend**](dir_53d62147b82bd29328805b2087bd1012.md) **>** [**visitors**](dir_007753111df00039ee3ec058cc286377.md) **>** [**geometry\_visitor.h**](geometry__visitor_8h.md)

[Go to the documentation of this file](geometry__visitor_8h.md)


```C++
#pragma once
#include <string>
#include <uipc/geometry/attribute_collection.h>
namespace uipc::geometry
{
class IGeometry;
}
namespace uipc::backend
{
class UIPC_CORE_API GeometryVisitor
{
  public:
    GeometryVisitor(geometry::IGeometry& geometry);
    void collect_attribute_collections(vector<std::string>& names,
                                       vector<geometry::AttributeCollection*>& collections);

  private:
    geometry::IGeometry& m_geometry;
};
}  // namespace uipc::backend
```


