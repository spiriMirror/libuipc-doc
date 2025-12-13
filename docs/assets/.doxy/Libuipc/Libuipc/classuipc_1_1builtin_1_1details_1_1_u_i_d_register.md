

# Class uipc::builtin::details::UIDRegister



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**builtin**](namespaceuipc_1_1builtin.md) **>** [**details**](namespaceuipc_1_1builtin_1_1details.md) **>** [**UIDRegister**](classuipc_1_1builtin_1_1details_1_1_u_i_d_register.md)










Inherited by the following classes: [uipc::builtin::ConstitutionUIDCollection](classuipc_1_1builtin_1_1_constitution_u_i_d_collection.md),  [uipc::builtin::ImplicitGeometryUIDCollection](classuipc_1_1builtin_1_1_implicit_geometry_u_i_d_collection.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  bool | [**exists**](#function-exists) (U64 uid) const<br> |
|  const [**UIDInfo**](structuipc_1_1builtin_1_1_u_i_d_info.md) & | [**find**](#function-find) (U64 uid) const<br> |
|  Json | [**to\_json**](#function-to_json) () noexcept const<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
|  void | [**create**](#function-create) (const [**UIDInfo**](structuipc_1_1builtin_1_1_u_i_d_info.md) & info, const [**CreatorInfo**](classuipc_1_1builtin_1_1details_1_1_u_i_d_register_1_1_creator_info.md) & creator) <br> |




## Public Functions Documentation




### function exists 

```C++
bool uipc::builtin::details::UIDRegister::exists (
    U64 uid
) const
```




<hr>



### function find 

```C++
const UIDInfo & uipc::builtin::details::UIDRegister::find (
    U64 uid
) const
```




<hr>



### function to\_json 

```C++
Json uipc::builtin::details::UIDRegister::to_json () noexcept const
```




<hr>
## Protected Functions Documentation




### function create 

```C++
void uipc::builtin::details::UIDRegister::create (
    const UIDInfo & info,
    const CreatorInfo & creator
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/builtin/uid_register.h`

