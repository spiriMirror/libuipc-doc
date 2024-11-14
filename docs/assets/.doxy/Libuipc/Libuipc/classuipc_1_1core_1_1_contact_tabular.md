

# Class uipc::core::ContactTabular



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ContactTabular**](#function-contacttabular-12) () noexcept<br> |
|   | [**ContactTabular**](#function-contacttabular-22) (const [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) &) = delete<br> |
|  std::span&lt; const [**ContactModel**](classuipc_1_1core_1_1_contact_model.md) &gt; | [**contact\_models**](#function-contact_models) () noexcept const<br> |
|  [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & | [**create**](#function-create) (std::string\_view name="") noexcept<br> |
|  [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & | [**default\_element**](#function-default_element) () noexcept<br> |
|  void | [**default\_model**](#function-default_model-12) (Float friction\_rate, Float resistance, const Json & config=default\_config()) noexcept<br> |
|  const [**ContactModel**](classuipc_1_1core_1_1_contact_model.md) & | [**default\_model**](#function-default_model-22) () noexcept const<br> |
|  SizeT | [**element\_count**](#function-element_count) () noexcept const<br> |
|  void | [**insert**](#function-insert) (const [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & L, const [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & R, Float friction\_rate, Float resistance, bool enable=true, const Json & config=default\_config()) <br> |
|  [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) & | [**operator=**](#function-operator) (const [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) &) = delete<br> |
|   | [**~ContactTabular**](#function-contacttabular) () noexcept<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Json | [**default\_config**](#function-default_config) () noexcept<br> |


























## Public Functions Documentation




### function ContactTabular [1/2]

```C++
uipc::core::ContactTabular::ContactTabular () noexcept
```




<hr>



### function ContactTabular [2/2]

```C++
uipc::core::ContactTabular::ContactTabular (
    const ContactTabular &
) = delete
```




<hr>



### function contact\_models 

```C++
std::span< const ContactModel > uipc::core::ContactTabular::contact_models () noexcept const
```




<hr>



### function create 

```C++
ContactElement & uipc::core::ContactTabular::create (
    std::string_view name=""
) noexcept
```




<hr>



### function default\_element 

```C++
ContactElement & uipc::core::ContactTabular::default_element () noexcept
```




<hr>



### function default\_model [1/2]

```C++
void uipc::core::ContactTabular::default_model (
    Float friction_rate,
    Float resistance,
    const Json & config=default_config()
) noexcept
```




<hr>



### function default\_model [2/2]

```C++
const ContactModel & uipc::core::ContactTabular::default_model () noexcept const
```




<hr>



### function element\_count 

```C++
SizeT uipc::core::ContactTabular::element_count () noexcept const
```




<hr>



### function insert 

```C++
void uipc::core::ContactTabular::insert (
    const ContactElement & L,
    const ContactElement & R,
    Float friction_rate,
    Float resistance,
    bool enable=true,
    const Json & config=default_config()
) 
```




<hr>



### function operator= 

```C++
ContactTabular & uipc::core::ContactTabular::operator= (
    const ContactTabular &
) = delete
```




<hr>



### function ~ContactTabular 

```C++
uipc::core::ContactTabular::~ContactTabular () noexcept
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::core::ContactTabular::default_config () noexcept
```




<hr>## Friends Documentation





### friend to\_json 

```C++
void uipc::core::ContactTabular::to_json (
    Json & j,
    const ContactTabular & ct
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/contact_tabular.h`
