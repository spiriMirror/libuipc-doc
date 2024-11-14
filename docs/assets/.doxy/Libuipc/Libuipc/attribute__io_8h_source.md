

# File attribute\_io.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**io**](dir_852854ea57a318f61c10cfed1155dbd7.md) **>** [**attribute\_io.h**](attribute__io_8h.md)

[Go to the documentation of this file](attribute__io_8h.md)


```C++
#pragma once
#include <uipc/common/dllexport.h>
#include <uipc/common/smart_pointer.h>
#include <uipc/geometry/attribute_slot.h>

namespace uipc::geometry
{
class UIPC_IO_API AttributeIO final
{
  public:
    class Interface;

    AttributeIO(std::string_view file);
    ~AttributeIO() noexcept;

    void read(std::string_view name, IAttributeSlot& slot);

  private:
    U<Interface> m_impl;
};

class UIPC_IO_API AttributeIOError : public Exception
{
  public:
    using Exception::Exception;
};
}  // namespace uipc::geometry
```


