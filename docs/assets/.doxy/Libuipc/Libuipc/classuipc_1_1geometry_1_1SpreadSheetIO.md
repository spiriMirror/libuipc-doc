

# Class uipc::geometry::SpreadSheetIO



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**SpreadSheetIO**](classuipc_1_1geometry_1_1SpreadSheetIO.md)



_A class for writing geometry spreadsheet._ [More...](#detailed-description)

* `#include <spread_sheet_io.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SpreadSheetIO**](#function-spreadsheetio) (std::string\_view output\_folder="./") <br> |
|  void | [**write\_csv**](#function-write_csv-12) (std::string\_view geo\_name, const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & geo) const<br> |
|  void | [**write\_csv**](#function-write_csv-22) (const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & geo) const<br> |
|  void | [**write\_json**](#function-write_json-12) (std::string\_view geo\_name, const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & geo) const<br> |
|  void | [**write\_json**](#function-write_json-22) (const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & geo) const<br> |




























## Detailed Description



```C++
SimplicialComplexIO io;
auto mesh = io.read("cube.msh");
SpreadSheetIO sio;
// dump to csv
sio.write_csv("spreadsheet", mesh);
// dump to json
sio.write_json("spreadsheet", mesh);
```
 


    
## Public Functions Documentation




### function SpreadSheetIO 

```C++
uipc::geometry::SpreadSheetIO::SpreadSheetIO (
    std::string_view output_folder="./"
) 
```




<hr>



### function write\_csv [1/2]

```C++
void uipc::geometry::SpreadSheetIO::write_csv (
    std::string_view geo_name,
    const Geometry & geo
) const
```




<hr>



### function write\_csv [2/2]

```C++
void uipc::geometry::SpreadSheetIO::write_csv (
    const Geometry & geo
) const
```




<hr>



### function write\_json [1/2]

```C++
void uipc::geometry::SpreadSheetIO::write_json (
    std::string_view geo_name,
    const Geometry & geo
) const
```




<hr>



### function write\_json [2/2]

```C++
void uipc::geometry::SpreadSheetIO::write_json (
    const Geometry & geo
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/io/spread_sheet_io.h`

