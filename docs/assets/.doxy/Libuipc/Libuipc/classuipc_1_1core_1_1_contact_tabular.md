

# Class uipc::core::ContactTabular



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ContactTabular**](#function-contacttabular-12) () noexcept<br> |
|   | [**ContactTabular**](#function-contacttabular-22) (const [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) &) = delete<br> |
|  [**ContactModel**](classuipc_1_1core_1_1_contact_model.md) | [**at**](#function-at) (SizeT i, SizeT j) const<br> |
|  ContactModelCollection | [**contact\_models**](#function-contact_models-12) () noexcept<br> |
|  CContactModelCollection | [**contact\_models**](#function-contact_models-22) () noexcept const<br> |
|  [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) | [**create**](#function-create) (std::string\_view name="") noexcept<br> |
|  [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) | [**create\_subscene**](#function-create_subscene) (std::string\_view name="") noexcept<br> |
|  [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) | [**default\_element**](#function-default_element) () noexcept<br> |
|  void | [**default\_model**](#function-default_model-12) (Float friction\_rate, Float resistance, bool enable=true, const Json & config=default\_config()) noexcept<br> |
|  [**ContactModel**](classuipc_1_1core_1_1_contact_model.md) | [**default\_model**](#function-default_model-22) () noexcept const<br> |
|  [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) | [**default\_subscene\_element**](#function-default_subscene_element) () noexcept<br> |
|  SizeT | [**element\_count**](#function-element_count) () noexcept const<br> |
|  IndexT | [**insert**](#function-insert) (const [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & L, const [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & R, Float friction\_rate, Float resistance, bool enable=true, const Json & config=default\_config()) <br> |
|  [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) & | [**operator=**](#function-operator) (const [**ContactTabular**](classuipc_1_1core_1_1_contact_tabular.md) &) = delete<br> |
|  ContactModelCollection | [**subscene\_contact\_models**](#function-subscene_contact_models-12) () noexcept<br> |
|  CContactModelCollection | [**subscene\_contact\_models**](#function-subscene_contact_models-22) () noexcept const<br> |
|  SizeT | [**subscene\_element\_count**](#function-subscene_element_count) () noexcept const<br> |
|  IndexT | [**subscene\_insert**](#function-subscene_insert) (const [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & L, const [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & R, bool enable=true, const Json & config=default\_config()) <br> |
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



### function at 

```C++
ContactModel uipc::core::ContactTabular::at (
    SizeT i,
    SizeT j
) const
```




<hr>



### function contact\_models [1/2]

```C++
ContactModelCollection uipc::core::ContactTabular::contact_models () noexcept
```




<hr>



### function contact\_models [2/2]

```C++
CContactModelCollection uipc::core::ContactTabular::contact_models () noexcept const
```




<hr>



### function create 

```C++
ContactElement uipc::core::ContactTabular::create (
    std::string_view name=""
) noexcept
```




<hr>



### function create\_subscene 

```C++
ContactElement uipc::core::ContactTabular::create_subscene (
    std::string_view name=""
) noexcept
```




<hr>



### function default\_element 

```C++
ContactElement uipc::core::ContactTabular::default_element () noexcept
```




<hr>



### function default\_model [1/2]

```C++
void uipc::core::ContactTabular::default_model (
    Float friction_rate,
    Float resistance,
    bool enable=true,
    const Json & config=default_config()
) noexcept
```




<hr>



### function default\_model [2/2]

```C++
ContactModel uipc::core::ContactTabular::default_model () noexcept const
```




<hr>



### function default\_subscene\_element 

```C++
ContactElement uipc::core::ContactTabular::default_subscene_element () noexcept
```




<hr>



### function element\_count 

```C++
SizeT uipc::core::ContactTabular::element_count () noexcept const
```




<hr>



### function insert 

```C++
IndexT uipc::core::ContactTabular::insert (
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



### function subscene\_contact\_models [1/2]

```C++
ContactModelCollection uipc::core::ContactTabular::subscene_contact_models () noexcept
```




<hr>



### function subscene\_contact\_models [2/2]

```C++
CContactModelCollection uipc::core::ContactTabular::subscene_contact_models () noexcept const
```




<hr>



### function subscene\_element\_count 

```C++
SizeT uipc::core::ContactTabular::subscene_element_count () noexcept const
```




<hr>



### function subscene\_insert 

```C++
IndexT uipc::core::ContactTabular::subscene_insert (
    const ContactElement & L,
    const ContactElement & R,
    bool enable=true,
    const Json & config=default_config()
) 
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





### friend Scene 

```C++
class uipc::core::ContactTabular::Scene (
    internal::Scene
) 
```




<hr>



### friend to\_json 

```C++
void uipc::core::ContactTabular::to_json (
    Json & j,
    const ContactTabular & ct
) 
```




<hr>



### friend ContactTabularVisitor 

```C++
class uipc::core::ContactTabular::ContactTabularVisitor (
    uipc::backend::ContactTabularVisitor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/contact_tabular.h`

