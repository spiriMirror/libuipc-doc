

# File scene\_io.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**io**](dir_852854ea57a318f61c10cfed1155dbd7.md) **>** [**scene\_io.h**](scene__io_8h.md)

[Go to the documentation of this file](scene__io_8h.md)


```C++
#pragma once
#include <uipc/core/scene.h>
#include <uipc/common/exception.h>
#include <uipc/geometry/simplicial_complex.h>

namespace uipc::core
{
class UIPC_IO_API SceneIO
{
  public:
    SceneIO(Scene& scene);

    void write_surface(std::string_view filename);

    geometry::SimplicialComplex simplicial_surface() const;
    geometry::SimplicialComplex simplicial_surface(IndexT dim) const;

  private:
    Scene& m_scene;
    void   write_surface_obj(std::string_view filename);
};

class UIPC_IO_API SceneIOError : public Exception
{
  public:
    using Exception::Exception;
};
}  // namespace uipc::core
```


