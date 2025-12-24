

# Class uipc::core::ConstitutionTabular



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ConstitutionTabular**](classuipc_1_1core_1_1ConstitutionTabular.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ConstitutionTabular**](#function-constitutiontabular-12) () noexcept<br> |
|   | [**ConstitutionTabular**](#function-constitutiontabular-22) (const [**ConstitutionTabular**](classuipc_1_1core_1_1ConstitutionTabular.md) &) = delete<br> |
|  void | [**insert**](#function-insert) (const [**constitution::IConstitution**](classuipc_1_1constitution_1_1IConstitution.md) & constitution) <br> |
|  [**ConstitutionTabular**](classuipc_1_1core_1_1ConstitutionTabular.md) & | [**operator=**](#function-operator) (const [**ConstitutionTabular**](classuipc_1_1core_1_1ConstitutionTabular.md) &) = delete<br> |
|  const set&lt; std::string &gt; & | [**types**](#function-types) () noexcept const<br> |
|  span&lt; U64 &gt; | [**uids**](#function-uids) () noexcept const<br> |
|   | [**~ConstitutionTabular**](#function-constitutiontabular) () noexcept<br> |




























## Public Functions Documentation




### function ConstitutionTabular [1/2]

```C++
uipc::core::ConstitutionTabular::ConstitutionTabular () noexcept
```




<hr>



### function ConstitutionTabular [2/2]

```C++
uipc::core::ConstitutionTabular::ConstitutionTabular (
    const ConstitutionTabular &
) = delete
```




<hr>



### function insert 

```C++
void uipc::core::ConstitutionTabular::insert (
    const constitution::IConstitution & constitution
) 
```




<hr>



### function operator= 

```C++
ConstitutionTabular & uipc::core::ConstitutionTabular::operator= (
    const ConstitutionTabular &
) = delete
```




<hr>



### function types 

```C++
const set< std::string > & uipc::core::ConstitutionTabular::types () noexcept const
```




<hr>



### function uids 

```C++
span< U64 > uipc::core::ConstitutionTabular::uids () noexcept const
```




<hr>



### function ~ConstitutionTabular 

```C++
uipc::core::ConstitutionTabular::~ConstitutionTabular () noexcept
```




<hr>## Friends Documentation





### friend Scene 

```C++
class uipc::core::ConstitutionTabular::Scene (
    internal::Scene
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/constitution_tabular.h`

