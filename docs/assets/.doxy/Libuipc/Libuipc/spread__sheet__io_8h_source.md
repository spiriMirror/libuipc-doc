

# File spread\_sheet\_io.h

[**File List**](files.md) **>** [**include**](dir_d44c64559bbebec7f509842c48db8b23.md) **>** [**uipc**](dir_9f30510905f1286cc334e7ecdb1aceca.md) **>** [**io**](dir_852854ea57a318f61c10cfed1155dbd7.md) **>** [**spread\_sheet\_io.h**](spread__sheet__io_8h.md)

[Go to the documentation of this file](spread__sheet__io_8h.md)


```C++
#pragma once
#include <uipc/geometry/simplicial_complex.h>
namespace uipc::geometry
{
class UIPC_IO_API SpreadSheetIO
{
  public:
    SpreadSheetIO(std::string_view output_folder = "./");
    void write_json(std::string_view geo_name, const SimplicialComplex& simplicial_complex) const;
    void write_json(const SimplicialComplex& simplicial_complex) const;
    void write_csv(std::string_view geo_name, const SimplicialComplex& simplicial_complex) const;
    void write_csv(const SimplicialComplex& simplicial_complex) const;

  private:
    string m_output_folder;
};
}  // namespace uipc::geometry
```


