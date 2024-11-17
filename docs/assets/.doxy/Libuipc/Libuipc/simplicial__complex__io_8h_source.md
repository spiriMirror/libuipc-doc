

# File simplicial\_complex\_io.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**io**](dir_852854ea57a318f61c10cfed1155dbd7.md) **>** [**simplicial\_complex\_io.h**](simplicial__complex__io_8h.md)

[Go to the documentation of this file](simplicial__complex__io_8h.md)


```C++
#pragma once
#include <uipc/common/exception.h>
#include <uipc/geometry/simplicial_complex.h>


namespace uipc::geometry
{
class UIPC_IO_API SimplicialComplexIO
{
  public:
    SimplicialComplexIO() = default;
    explicit SimplicialComplexIO(const Matrix4x4& pre_transform) noexcept;
    explicit SimplicialComplexIO(const Transform& pre_transform) noexcept;

    // default copy/move ctor/assignment
    SimplicialComplexIO(const SimplicialComplexIO&)            = default;
    SimplicialComplexIO(SimplicialComplexIO&&)                 = default;
    SimplicialComplexIO& operator=(const SimplicialComplexIO&) = default;
    SimplicialComplexIO& operator=(SimplicialComplexIO&&)      = default;

    [[nodiscard]] SimplicialComplex read(std::string_view file_name);

    [[nodiscard]] SimplicialComplex read_msh(std::string_view file_name);

    [[nodiscard]] SimplicialComplex read_obj(std::string_view file_name);


    void write(std::string_view file_name, const SimplicialComplex& sc);

    void write_obj(std::string_view file_name, const SimplicialComplex& sc);

    void write_msh(std::string_view file_name, const SimplicialComplex& sc);

  private:
    Matrix4x4 m_pre_transform = Matrix4x4::Identity();
    void      apply_pre_transform(Vector3& v) const noexcept;
};
}  // namespace uipc::geometry

namespace uipc::geometry
{
class GeometryIOError : public Exception
{
  public:
    using Exception::Exception;
};
}  // namespace uipc::geometry
```


