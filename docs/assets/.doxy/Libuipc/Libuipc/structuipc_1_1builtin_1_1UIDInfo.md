

# Struct uipc::builtin::UIDInfo



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**builtin**](namespaceuipc_1_1builtin.md) **>** [**UIDInfo**](structuipc_1_1builtin_1_1UIDInfo.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  string | [**author**](#variable-author)  <br> |
|  string | [**description**](#variable-description)  <br> |
|  string | [**email**](#variable-email)  <br> |
|  Json | [**extras**](#variable-extras)  <br> |
|  string | [**name**](#variable-name)  <br> |
|  string | [**type**](#variable-type)  <br> |
|  U64 | [**uid**](#variable-uid)   = `0`<br> |
|  string | [**website**](#variable-website)  <br> |


## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  constexpr U64 | [**OfficialBuiltinUIDStart**](#variable-officialbuiltinuidstart)   = `0`<br> |
|  constexpr U64 | [**UserDefinedUIDStart**](#variable-userdefineduidstart)   = `1ull &lt;&lt; 32`<br> |














## Public Functions

| Type | Name |
| ---: | :--- |
|  bool | [**is\_official\_builtin\_uid**](#function-is_official_builtin_uid) (U64 uid) noexcept const<br> |
|  bool | [**is\_user\_defined\_uid**](#function-is_user_defined_uid) (U64 uid) noexcept const<br> |
|  Json | [**to\_json**](#function-to_json) () noexcept const<br> |




























## Public Attributes Documentation




### variable author 

```C++
string uipc::builtin::UIDInfo::author;
```




<hr>



### variable description 

```C++
string uipc::builtin::UIDInfo::description;
```




<hr>



### variable email 

```C++
string uipc::builtin::UIDInfo::email;
```




<hr>



### variable extras 

```C++
Json uipc::builtin::UIDInfo::extras;
```




<hr>



### variable name 

```C++
string uipc::builtin::UIDInfo::name;
```




<hr>



### variable type 

```C++
string uipc::builtin::UIDInfo::type;
```




<hr>



### variable uid 

```C++
U64 uipc::builtin::UIDInfo::uid;
```




<hr>



### variable website 

```C++
string uipc::builtin::UIDInfo::website;
```




<hr>
## Public Static Attributes Documentation




### variable OfficialBuiltinUIDStart 

```C++
constexpr U64 uipc::builtin::UIDInfo::OfficialBuiltinUIDStart;
```




<hr>



### variable UserDefinedUIDStart 

```C++
constexpr U64 uipc::builtin::UIDInfo::UserDefinedUIDStart;
```




<hr>
## Public Functions Documentation




### function is\_official\_builtin\_uid 

```C++
bool uipc::builtin::UIDInfo::is_official_builtin_uid (
    U64 uid
) noexcept const
```




<hr>



### function is\_user\_defined\_uid 

```C++
bool uipc::builtin::UIDInfo::is_user_defined_uid (
    U64 uid
) noexcept const
```




<hr>



### function to\_json 

```C++
Json uipc::builtin::UIDInfo::to_json () noexcept const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/builtin/uid_info.h`

