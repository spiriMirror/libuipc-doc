

# Class uipc::core::SanityCheckMessage



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SanityCheckMessage**](classuipc_1_1core_1_1_sanity_check_message.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SanityCheckMessage**](#function-sanitycheckmessage) () = default<br> |
|  const unordered\_map&lt; std::string, S&lt; [**geometry::Geometry**](classuipc_1_1geometry_1_1_geometry.md) &gt; &gt; & | [**geometries**](#function-geometries) () noexcept const<br> |
|  U64 | [**id**](#function-id) () noexcept const<br> |
|  bool | [**is\_empty**](#function-is_empty) () noexcept const<br> |
|  std::string\_view | [**message**](#function-message) () noexcept const<br> |
|  std::string\_view | [**name**](#function-name) () noexcept const<br> |
|  SanityCheckResult | [**result**](#function-result) () noexcept const<br> |




























## Public Functions Documentation




### function SanityCheckMessage 

```C++
uipc::core::SanityCheckMessage::SanityCheckMessage () = default
```




<hr>



### function geometries 

```C++
const unordered_map< std::string, S< geometry::Geometry > > & uipc::core::SanityCheckMessage::geometries () noexcept const
```




<hr>



### function id 

```C++
U64 uipc::core::SanityCheckMessage::id () noexcept const
```




<hr>



### function is\_empty 

```C++
bool uipc::core::SanityCheckMessage::is_empty () noexcept const
```




<hr>



### function message 

```C++
std::string_view uipc::core::SanityCheckMessage::message () noexcept const
```




<hr>



### function name 

```C++
std::string_view uipc::core::SanityCheckMessage::name () noexcept const
```




<hr>



### function result 

```C++
SanityCheckResult uipc::core::SanityCheckMessage::result () noexcept const
```




<hr>## Friends Documentation





### friend SanityCheckMessageVisitor 

```C++
class uipc::core::SanityCheckMessage::SanityCheckMessageVisitor (
    backend::SanityCheckMessageVisitor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/i_sanity_checker.h`

