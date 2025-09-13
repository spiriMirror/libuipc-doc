

# File urdf\_io.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**io**](dir_852854ea57a318f61c10cfed1155dbd7.md) **>** [**urdf\_io.h**](urdf__io_8h.md)

[Go to the documentation of this file](urdf__io_8h.md)


```C++
#include <uipc/common/type_define.h>
#include <uipc/common/smart_pointer.h>
#include <uipc/core/object.h>
#include <uipc/geometry/implicit_geometry_slot.h>
#include <uipc/geometry/simplicial_complex_slot.h>
namespace uipc::io
{
class UIPC_IO_API UrdfController
{
    class Impl;
    friend class UrdfIO;

  public:
    ~UrdfController();
    void move_root(const Vector3& xyz, const Vector3& rpy) const;
    void rotate_to(std::string_view joint_name, Float angle) const;
    void apply_to(std::string_view attr) const;
    S<geometry::ImplicitGeometrySlot>          revolute_joints() const;
    vector<S<geometry::SimplicialComplexSlot>> links() const;
    void                                       sync_visual_mesh() const;
    // copy constructor
    UrdfController(const UrdfController& other);
    UrdfController(UrdfController&& other) = default;

  private:
    UrdfController(S<Impl> impl);
    S<Impl> m_impl;
};

class UIPC_IO_API UrdfIO
{
    class Impl;

  public:
    UrdfIO(const Json& config = UrdfIO::default_config());
    ~UrdfIO();

    UrdfController read(uipc::core::Object& object, std::string_view urdf_path);
    static Json    default_config();

  private:
    U<Impl> m_impl;
};

class UIPC_IO_API UrdfIOError : public Exception
{
  public:
    using Exception::Exception;
};
}  // namespace uipc::io
```


