

# Class uipc::constitution::IConstitution



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**IConstitution**](classuipc_1_1constitution_1_1IConstitution.md)










Inherited by the following classes: [uipc::constitution::AffineBodyConstitution](classuipc_1_1constitution_1_1AffineBodyConstitution.md),  [uipc::constitution::AffineBodyExternalBodyForce](classuipc_1_1constitution_1_1AffineBodyExternalBodyForce.md),  [uipc::constitution::Constraint](classuipc_1_1constitution_1_1Constraint.md),  [uipc::constitution::FiniteElementConstitution](classuipc_1_1constitution_1_1FiniteElementConstitution.md),  [uipc::constitution::FiniteElementExtraConstitution](classuipc_1_1constitution_1_1FiniteElementExtraConstitution.md),  [uipc::constitution::InterAffineBodyConstitution](classuipc_1_1constitution_1_1InterAffineBodyConstitution.md),  [uipc::constitution::InterPrimitiveConstitution](classuipc_1_1constitution_1_1InterPrimitiveConstitution.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**name**](#function-name) () noexcept const<br> |
|  std::string\_view | [**type**](#function-type) () noexcept const<br> |
|  U64 | [**uid**](#function-uid) () noexcept const<br> |
|  const [**builtin::UIDInfo**](structuipc_1_1builtin_1_1UIDInfo.md) & | [**uid\_info**](#function-uid_info) () noexcept const<br> |
| virtual  | [**~IConstitution**](#function-iconstitution) () = default<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](#function-get_uid) () noexcept const = 0<br> |




## Public Functions Documentation




### function name 

```C++
std::string_view uipc::constitution::IConstitution::name () noexcept const
```




<hr>



### function type 

```C++
std::string_view uipc::constitution::IConstitution::type () noexcept const
```




<hr>



### function uid 

```C++
U64 uipc::constitution::IConstitution::uid () noexcept const
```




<hr>



### function uid\_info 

```C++
const builtin::UIDInfo & uipc::constitution::IConstitution::uid_info () noexcept const
```




<hr>



### function ~IConstitution 

```C++
virtual uipc::constitution::IConstitution::~IConstitution () = default
```




<hr>
## Protected Functions Documentation




### function get\_uid 

```C++
virtual U64 uipc::constitution::IConstitution::get_uid () noexcept const = 0
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/constitution.h`

