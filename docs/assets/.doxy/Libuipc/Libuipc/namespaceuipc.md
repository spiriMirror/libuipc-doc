

# Namespace uipc



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**backend**](namespaceuipc_1_1backend.md) <br> |
| namespace | [**builtin**](namespaceuipc_1_1builtin.md) <br> |
| namespace | [**constitution**](namespaceuipc_1_1constitution.md) <br> |
| namespace | [**core**](namespaceuipc_1_1core.md) <br> |
| namespace | [**details**](namespaceuipc_1_1details.md) <br> |
| namespace | [**diff\_sim**](namespaceuipc_1_1diff__sim.md) <br> |
| namespace | [**geometry**](namespaceuipc_1_1geometry.md) <br> |
| namespace | [**gui**](namespaceuipc_1_1gui.md) <br> |
| namespace | [**pmr**](namespaceuipc_1_1pmr.md) <br> |
| namespace | [**sanity\_check**](namespaceuipc_1_1sanity__check.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**BufferInfo**](classuipc_1_1_buffer_info.md) <br> |
| class | [**Exception**](classuipc_1_1_exception.md) <br> |
| class | [**GlobalTimer**](classuipc_1_1_global_timer.md) <br> |
| class | [**JsonIOError**](classuipc_1_1_json_i_o_error.md) <br> |
| class | [**LogPatternGuard**](classuipc_1_1_log_pattern_guard.md) <br> |
| struct | [**PmrDeleter**](structuipc_1_1_pmr_deleter.md) &lt;typename T&gt;<br> |
| class | [**Timer**](classuipc_1_1_timer.md) <br> |
| class | [**is\_matrix**](classuipc_1_1is__matrix.md) &lt;typename MatrixT&gt;<br> |
| class | [**is\_matrix&lt; Eigen::Matrix&lt; Scalar, Rows, Cols, Options, MaxRows, MaxCols &gt; &gt;**](classuipc_1_1is__matrix_3_01_eigen_1_1_matrix_3_01_scalar_00_01_rows_00_01_cols_00_01_options_00209f23989f4c2eaf53edf139526fd2cf.md) &lt;typename Scalar, Rows, Cols, Options, MaxRows, MaxCols&gt;<br> |
| struct | [**propagate\_const**](structuipc_1_1propagate__const.md) &lt;typename T, typename DstT&gt;<br> |
| struct | [**signature**](structuipc_1_1signature.md) &lt;typename Sig&gt;<br> |
| struct | [**signature&lt; R(&)(Args...)&gt;**](structuipc_1_1signature_3_01_r_07_6_08_07_args_8_8_8_08_4.md) &lt;typename R, Args&gt;<br> |
| struct | [**signature&lt; R(\*)(Args...)&gt;**](structuipc_1_1signature_3_01_r_07_5_08_07_args_8_8_8_08_4.md) &lt;typename R, Args&gt;<br> |
| struct | [**signature&lt; R(Args...)&gt;**](structuipc_1_1signature_3_01_r_07_args_8_8_8_08_4.md) &lt;typename R, Args&gt;<br> |
| struct | [**signature&lt; R(C::\*)(Args...) && &gt;**](structuipc_1_1signature_3_01_r_07_c_1_1_5_08_07_args_8_8_8_08_01_6_6_01_4.md) &lt;typename R, typename C, Args&gt;<br> |
| struct | [**signature&lt; R(C::\*)(Args...) const &gt;**](structuipc_1_1signature_3_01_r_07_c_1_1_5_08_07_args_8_8_8_08_01const_01_4.md) &lt;typename R, typename C, Args&gt;<br> |
| struct | [**signature&lt; R(C::\*)(Args...) const volatile &gt;**](structuipc_1_1signature_3_01_r_07_c_1_1_5_08_07_args_8_8_8_08_01const_01volatile_01_4.md) &lt;typename R, typename C, Args&gt;<br> |
| struct | [**signature&lt; R(C::\*)(Args...) volatile &gt;**](structuipc_1_1signature_3_01_r_07_c_1_1_5_08_07_args_8_8_8_08_01volatile_01_4.md) &lt;typename R, typename C, Args&gt;<br> |
| struct | [**signature&lt; R(C::\*)(Args...)&gt;**](structuipc_1_1signature_3_01_r_07_c_1_1_5_08_07_args_8_8_8_08_4.md) &lt;typename R, typename C, Args&gt;<br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::pmr::polymorphic\_allocator&lt; T &gt; | [**Allocator**](#typedef-allocator)  <br> |
| typedef Eigen::AngleAxis&lt; Float &gt; | [**AngleAxis**](#typedef-angleaxis)  <br> |
| typedef double | [**Float**](#typedef-float)  <br> |
| typedef int32\_t | [**I32**](#typedef-i32)  <br> |
| typedef int64\_t | [**I64**](#typedef-i64)  <br> |
| typedef int32\_t | [**IndexT**](#typedef-indext)  <br> |
| typedef nlohmann::json | [**Json**](#typedef-json)  <br> |
| typedef Matrix&lt; Float, 12, 12 &gt; | [**Matrix12x12**](#typedef-matrix12x12)  <br> |
| typedef Matrix&lt; Float, 2, 2 &gt; | [**Matrix2x2**](#typedef-matrix2x2)  <br> |
| typedef Matrix&lt; Float, 3, 3 &gt; | [**Matrix3x3**](#typedef-matrix3x3)  <br> |
| typedef Matrix&lt; Float, 4, 4 &gt; | [**Matrix4x4**](#typedef-matrix4x4)  <br> |
| typedef Matrix&lt; Float, 6, 6 &gt; | [**Matrix6x6**](#typedef-matrix6x6)  <br> |
| typedef Matrix&lt; Float, 9, 9 &gt; | [**Matrix9x9**](#typedef-matrix9x9)  <br> |
| typedef Eigen::MatrixX&lt; Float &gt; | [**MatrixX**](#typedef-matrixx)  <br> |
| typedef Eigen::Quaternion&lt; Float &gt; | [**Quaternion**](#typedef-quaternion)  <br> |
| typedef std::shared\_ptr&lt; T &gt; | [**S**](#typedef-s)  <br> |
| typedef std::size\_t | [**SizeT**](#typedef-sizet)  <br> |
| typedef Eigen::Transform&lt; Float, 3, Eigen::Affine &gt; | [**Transform**](#typedef-transform)  <br> |
| typedef Eigen::Translation&lt; Float, 3 &gt; | [**Translation**](#typedef-translation)  <br> |
| typedef std::unique\_ptr&lt; T, [**PmrDeleter**](structuipc_1_1_pmr_deleter.md)&lt; T &gt; &gt; | [**U**](#typedef-u)  <br> |
| typedef uint32\_t | [**U32**](#typedef-u32)  <br> |
| typedef uint64\_t | [**U64**](#typedef-u64)  <br> |
| typedef Vector&lt; Float, 12 &gt; | [**Vector12**](#typedef-vector12)  <br> |
| typedef Vector&lt; Float, 2 &gt; | [**Vector2**](#typedef-vector2)  <br> |
| typedef Vector&lt; IndexT, 2 &gt; | [**Vector2i**](#typedef-vector2i)  <br> |
| typedef Vector&lt; Float, 3 &gt; | [**Vector3**](#typedef-vector3)  <br> |
| typedef Vector&lt; IndexT, 3 &gt; | [**Vector3i**](#typedef-vector3i)  <br> |
| typedef Vector&lt; Float, 4 &gt; | [**Vector4**](#typedef-vector4)  <br> |
| typedef Vector&lt; IndexT, 4 &gt; | [**Vector4i**](#typedef-vector4i)  <br> |
| typedef Vector&lt; Float, 6 &gt; | [**Vector6**](#typedef-vector6)  <br> |
| typedef Vector&lt; Float, 9 &gt; | [**Vector9**](#typedef-vector9)  <br> |
| typedef Eigen::VectorX&lt; Float &gt; | [**VectorX**](#typedef-vectorx)  <br> |
| typedef Eigen::VectorX&lt; IndexT &gt; | [**VectorXi**](#typedef-vectorxi)  <br> |
| typedef Eigen::VectorX&lt; I64 &gt; | [**VectorXi64**](#typedef-vectorxi64)  <br> |
| typedef Eigen::VectorX&lt; U32 &gt; | [**VectorXu**](#typedef-vectorxu)  <br> |
| typedef Eigen::VectorX&lt; U64 &gt; | [**VectorXu64**](#typedef-vectorxu64)  <br> |
| typedef std::weak\_ptr&lt; T &gt; | [**W**](#typedef-w)  <br> |
| typedef typename [**propagate\_const**](structuipc_1_1propagate__const.md)&lt; T, DstT &gt;::type | [**propagate\_const\_t**](#typedef-propagate_const_t)  <br> |
| typedef typename [**signature**](structuipc_1_1signature.md)&lt; Sig &gt;::type | [**signature\_t**](#typedef-signature_t)  <br> |
| typedef std::stack&lt; T, std::pmr::deque&lt; T &gt; &gt; | [**stack**](#typedef-stack)  <br> |




## Public Attributes

| Type | Name |
| ---: | :--- |
|  bool | [**RUNTIME\_CHECK**](#variable-runtime_check)   = `false`<br> |
|  bool | [**is\_matrix\_v**](#variable-is_matrix_v)   = `[**is\_matrix**](classuipc_1_1is__matrix.md)&lt;MatrixT&gt;::value`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (I32) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (U32) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (I64) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (U64) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Vector2) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Vector3) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Vector4) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Vector2i) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Vector3i) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Vector4i) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Vector6) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Vector9) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Vector12) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Matrix2x2) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Matrix3x3) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Matrix4x4) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Matrix6x6) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Matrix9x9) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (Matrix12x12) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (VectorX) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (VectorXi) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (VectorXi64) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (VectorXu) <br> |
|   | [**READABLE\_TYPE\_NAME\_AS\_ALIAS**](#function-readable_type_name_as_alias) (VectorXu64) <br> |
|  UIPC\_CORE\_API void | [**abort**](#function-abort) () noexcept<br> |
|  auto | [**as\_eigen**](#function-as_eigen) (span&lt; T &gt; s) <br> |
|  UIPC\_CORE\_API const Json & | [**config**](#function-config) () <br> |
|  UIPC\_CORE\_API Json | [**default\_config**](#function-default_config) () <br> |
|  UIPC\_CORE\_API std::string | [**demangle**](#function-demangle) (const std::string & mangled\_name) <br> |
|  std::string | [**demangle**](#function-demangle) () noexcept<br> |
|  size\_t | [**encode\_offset\_count**](#function-encode_offset_count) (RandIt first, RandIt last, OffsetCountIt offsets, OffsetCountIt counts, Pred && pred) <br> |
|  auto | [**encode\_offset\_count**](#function-encode_offset_count) (RandIt first, RandIt last, OffsetCountIt offset, OffsetCountIt count) <br> |
|  UIPC\_CORE\_API void | [**init**](#function-init) (const Json & config) <br> |
|  S&lt; T &gt; | [**make\_shared**](#function-make_shared) (Args &&... args) <br> |
|  U&lt; T &gt; | [**make\_unique**](#function-make_unique) (Args &&... args) <br> |
|  long double | [**operator""\_GPa**](#function-operator""_gpa) (long double value) <br>_Pascal literal operator (GPa)_  |
|  long double | [**operator""\_MPa**](#function-operator""_mpa) (long double value) <br>_Pascal literal operator (MPa)_  |
|  long double | [**operator""\_N**](#function-operator""_n) (long double value) <br>_Newton literal operator._  |
|  long double | [**operator""\_Pa**](#function-operator""_pa) (long double value) <br>_Pascal literal operator._  |
|  long double | [**operator""\_kPa**](#function-operator""_kpa) (long double value) <br>_Pascal literal operator (kPa)_  |
|  long double | [**operator""\_km**](#function-operator""_km) (long double value) <br>_Meter literal operator (km)_  |
|  long double | [**operator""\_m**](#function-operator""_m) (long double value) <br>_Meter literal operator._  |
|  long double | [**operator""\_mm**](#function-operator""_mm) (long double value) <br>_Meter literal operator (mm)_  |
|  long double | [**operator""\_ms**](#function-operator""_ms) (long double value) <br>_Second literal operator (ms)_  |
|  long double | [**operator""\_s**](#function-operator""_s) (long double value) <br>_Second literal operator._  |
|  std::string | [**readable\_type\_name**](#function-readable_type_name) () noexcept<br> |
|  std::string | [**readable\_type\_name&lt; double &gt;**](#function-readable_type_name<-double->) () noexcept<br> |
|  std::string | [**readable\_type\_name&lt; float &gt;**](#function-readable_type_name<-float->) () noexcept<br> |
|  std::string | [**readable\_type\_name&lt; std::string &gt;**](#function-readable_type_name<-std::string->) () noexcept<br> |
|  std::size\_t | [**run\_length\_encode**](#function-run_length_encode) (InputIt in\_first, InputIt in\_last, OutputIt out\_unique, OutputCountIt out\_counts, Pred && pred) <br>_Run-length encode the input range, the input range must be sorted._  |
|  auto | [**run\_length\_encode**](#function-run_length_encode) (InputIt in\_first, InputIt in\_last, OutputIt out\_unique, OutputCountIt out\_counts) <br> |
|  U&lt; DstT &gt; | [**static\_pointer\_cast**](#function-static_pointer_cast) (U&lt; SrcT &gt; && src) <br> |
|  UIPC\_IO\_API int | [**test\_gltf**](#function-test_gltf) (std::string\_view path) <br> |




























## Public Types Documentation




### typedef Allocator 

```C++
using uipc::Allocator =  std::pmr::polymorphic_allocator<T>;
```




<hr>



### typedef AngleAxis 

```C++
using uipc::AngleAxis =  Eigen::AngleAxis<Float>;
```




<hr>



### typedef Float 

```C++
using uipc::Float =  double;
```




<hr>



### typedef I32 

```C++
using uipc::I32 =  int32_t;
```




<hr>



### typedef I64 

```C++
using uipc::I64 =  int64_t;
```




<hr>



### typedef IndexT 

```C++
using uipc::IndexT =  int32_t;
```




<hr>



### typedef Json 

```C++
using uipc::Json =  nlohmann::json;
```




<hr>



### typedef Matrix12x12 

```C++
using uipc::Matrix12x12 =  Matrix<Float, 12, 12>;
```




<hr>



### typedef Matrix2x2 

```C++
using uipc::Matrix2x2 =  Matrix<Float, 2, 2>;
```




<hr>



### typedef Matrix3x3 

```C++
using uipc::Matrix3x3 =  Matrix<Float, 3, 3>;
```




<hr>



### typedef Matrix4x4 

```C++
using uipc::Matrix4x4 =  Matrix<Float, 4, 4>;
```




<hr>



### typedef Matrix6x6 

```C++
using uipc::Matrix6x6 =  Matrix<Float, 6, 6>;
```




<hr>



### typedef Matrix9x9 

```C++
using uipc::Matrix9x9 =  Matrix<Float, 9, 9>;
```




<hr>



### typedef MatrixX 

```C++
using uipc::MatrixX =  Eigen::MatrixX<Float>;
```




<hr>



### typedef Quaternion 

```C++
using uipc::Quaternion =  Eigen::Quaternion<Float>;
```




<hr>



### typedef S 

```C++
using uipc::S =  std::shared_ptr<T>;
```




<hr>



### typedef SizeT 

```C++
using uipc::SizeT =  std::size_t;
```




<hr>



### typedef Transform 

```C++
using uipc::Transform =  Eigen::Transform<Float, 3, Eigen::Affine>;
```




<hr>



### typedef Translation 

```C++
using uipc::Translation =  Eigen::Translation<Float, 3>;
```




<hr>



### typedef U 

```C++
using uipc::U =  std::unique_ptr<T, PmrDeleter<T>>;
```




<hr>



### typedef U32 

```C++
using uipc::U32 =  uint32_t;
```




<hr>



### typedef U64 

```C++
using uipc::U64 =  uint64_t;
```




<hr>



### typedef Vector12 

```C++
using uipc::Vector12 =  Vector<Float, 12>;
```




<hr>



### typedef Vector2 

```C++
using uipc::Vector2 =  Vector<Float, 2>;
```




<hr>



### typedef Vector2i 

```C++
using uipc::Vector2i =  Vector<IndexT, 2>;
```




<hr>



### typedef Vector3 

```C++
using uipc::Vector3 =  Vector<Float, 3>;
```




<hr>



### typedef Vector3i 

```C++
using uipc::Vector3i =  Vector<IndexT, 3>;
```




<hr>



### typedef Vector4 

```C++
using uipc::Vector4 =  Vector<Float, 4>;
```




<hr>



### typedef Vector4i 

```C++
using uipc::Vector4i =  Vector<IndexT, 4>;
```




<hr>



### typedef Vector6 

```C++
using uipc::Vector6 =  Vector<Float, 6>;
```




<hr>



### typedef Vector9 

```C++
using uipc::Vector9 =  Vector<Float, 9>;
```




<hr>



### typedef VectorX 

```C++
using uipc::VectorX =  Eigen::VectorX<Float>;
```




<hr>



### typedef VectorXi 

```C++
using uipc::VectorXi =  Eigen::VectorX<IndexT>;
```




<hr>



### typedef VectorXi64 

```C++
using uipc::VectorXi64 =  Eigen::VectorX<I64>;
```




<hr>



### typedef VectorXu 

```C++
using uipc::VectorXu =  Eigen::VectorX<U32>;
```




<hr>



### typedef VectorXu64 

```C++
using uipc::VectorXu64 =  Eigen::VectorX<U64>;
```




<hr>



### typedef W 

```C++
using uipc::W =  std::weak_ptr<T>;
```




<hr>



### typedef propagate\_const\_t 

```C++
using uipc::propagate_const_t =  typename propagate_const<T, DstT>::type;
```




<hr>



### typedef signature\_t 

```C++
using uipc::signature_t =  typename signature<Sig>::type;
```




<hr>



### typedef stack 

```C++
using uipc::stack =  std::stack<T, std::pmr::deque<T>>;
```




<hr>
## Public Attributes Documentation




### variable RUNTIME\_CHECK 

```C++
bool uipc::RUNTIME_CHECK;
```




<hr>



### variable is\_matrix\_v 

```C++
bool uipc::is_matrix_v;
```




<hr>
## Public Functions Documentation




### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    I32
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    U32
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    I64
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    U64
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Vector2
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Vector3
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Vector4
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Vector2i
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Vector3i
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Vector4i
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Vector6
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Vector9
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Vector12
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Matrix2x2
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Matrix3x3
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Matrix4x4
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Matrix6x6
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Matrix9x9
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    Matrix12x12
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    VectorX
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    VectorXi
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    VectorXi64
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    VectorXu
) 
```




<hr>



### function READABLE\_TYPE\_NAME\_AS\_ALIAS 

```C++
uipc::READABLE_TYPE_NAME_AS_ALIAS (
    VectorXu64
) 
```




<hr>



### function abort 

```C++
UIPC_CORE_API void uipc::abort () noexcept
```




<hr>



### function as\_eigen 

```C++
template<std::floating_point T>
inline auto uipc::as_eigen (
    span< T > s
) 
```




<hr>



### function config 

```C++
UIPC_CORE_API const Json & uipc::config () 
```




<hr>



### function default\_config 

```C++
UIPC_CORE_API Json uipc::default_config () 
```




<hr>



### function demangle 

```C++
UIPC_CORE_API std::string uipc::demangle (
    const std::string & mangled_name
) 
```




<hr>



### function demangle 

```C++
template<typename T>
inline std::string uipc::demangle () noexcept
```




<hr>



### function encode\_offset\_count 

```C++
template<typename RandIt, typename OffsetCountIt, typename Pred>
size_t uipc::encode_offset_count (
    RandIt first,
    RandIt last,
    OffsetCountIt offsets,
    OffsetCountIt counts,
    Pred && pred
) 
```




<hr>



### function encode\_offset\_count 

```C++
template<typename RandIt, typename OffsetCountIt>
auto uipc::encode_offset_count (
    RandIt first,
    RandIt last,
    OffsetCountIt offset,
    OffsetCountIt count
) 
```




<hr>



### function init 

```C++
UIPC_CORE_API void uipc::init (
    const Json & config
) 
```




<hr>



### function make\_shared 

```C++
template<typename T, typename... Args>
S< T > uipc::make_shared (
    Args &&... args
) 
```




<hr>



### function make\_unique 

```C++
template<typename T, typename... Args>
U< T > uipc::make_unique (
    Args &&... args
) 
```




<hr>



### function operator""\_GPa 

_Pascal literal operator (GPa)_ 
```C++
long double uipc::operator""_GPa (
    long double value
) 
```




<hr>



### function operator""\_MPa 

_Pascal literal operator (MPa)_ 
```C++
long double uipc::operator""_MPa (
    long double value
) 
```




<hr>



### function operator""\_N 

_Newton literal operator._ 
```C++
long double uipc::operator""_N (
    long double value
) 
```




```C++
auto force = 1.0_N;
```
 


        

<hr>



### function operator""\_Pa 

_Pascal literal operator._ 
```C++
long double uipc::operator""_Pa (
    long double value
) 
```




```C++
auto pressure = 1.0_Pa;
```
 


        

<hr>



### function operator""\_kPa 

_Pascal literal operator (kPa)_ 
```C++
long double uipc::operator""_kPa (
    long double value
) 
```




<hr>



### function operator""\_km 

_Meter literal operator (km)_ 
```C++
long double uipc::operator""_km (
    long double value
) 
```




<hr>



### function operator""\_m 

_Meter literal operator._ 
```C++
long double uipc::operator""_m (
    long double value
) 
```




```C++
auto length = 1.0_m;
```
 


        

<hr>



### function operator""\_mm 

_Meter literal operator (mm)_ 
```C++
long double uipc::operator""_mm (
    long double value
) 
```




<hr>



### function operator""\_ms 

_Second literal operator (ms)_ 
```C++
long double uipc::operator""_ms (
    long double value
) 
```




<hr>



### function operator""\_s 

_Second literal operator._ 
```C++
long double uipc::operator""_s (
    long double value
) 
```




* 
* `cpp`
* `auto time = 1.0_s; *` 




        

<hr>



### function readable\_type\_name 

```C++
template<typename T>
inline std::string uipc::readable_type_name () noexcept
```




<hr>



### function readable\_type\_name&lt; double &gt; 

```C++
template<>
inline std::string uipc::readable_type_name< double > () noexcept
```




<hr>



### function readable\_type\_name&lt; float &gt; 

```C++
template<>
inline std::string uipc::readable_type_name< float > () noexcept
```




<hr>



### function readable\_type\_name&lt; std::string &gt; 

```C++
template<>
inline std::string uipc::readable_type_name< std::string > () noexcept
```




<hr>



### function run\_length\_encode 

_Run-length encode the input range, the input range must be sorted._ 
```C++
template<typename InputIt, typename OutputIt, typename OutputCountIt, typename Pred>
std::size_t uipc::run_length_encode (
    InputIt in_first,
    InputIt in_last,
    OutputIt out_unique,
    OutputCountIt out_counts,
    Pred && pred
) 
```





**Parameters:**


* `in_first` Input iterator to the beginning of the input range 
* `in_last` Input iterator to the end of the input range 
* `out_unique` Output iterator to the beginning of the unique values 
* `out_counts` Output iterator to the beginning of the counts of the unique values



**Returns:**

std::size\_t The number of unique values 





        

<hr>



### function run\_length\_encode 

```C++
template<typename InputIt, typename OutputIt, typename OutputCountIt>
auto uipc::run_length_encode (
    InputIt in_first,
    InputIt in_last,
    OutputIt out_unique,
    OutputCountIt out_counts
) 
```




<hr>



### function static\_pointer\_cast 

```C++
template<typename DstT, typename SrcT>
U< DstT > uipc::static_pointer_cast (
    U< SrcT > && src
) 
```




<hr>



### function test\_gltf 

```C++
UIPC_IO_API int uipc::test_gltf (
    std::string_view path
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/backend/buffer.h`

