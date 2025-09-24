

# Class uipc::core::SubsceneTabular



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SubsceneTabular**](classuipc_1_1core_1_1_subscene_tabular.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SubsceneTabular**](#function-subscenetabular-12) () noexcept<br> |
|   | [**SubsceneTabular**](#function-subscenetabular-22) (const [**SubsceneTabular**](classuipc_1_1core_1_1_subscene_tabular.md) &) = delete<br> |
|  [**SubsceneModel**](classuipc_1_1core_1_1_subscene_model.md) | [**at**](#function-at) (SizeT i, SizeT j) const<br> |
|  [**SubsceneElement**](classuipc_1_1core_1_1_subscene_element.md) | [**create**](#function-create) (std::string\_view name="") noexcept<br> |
|  [**SubsceneElement**](classuipc_1_1core_1_1_subscene_element.md) | [**default\_element**](#function-default_element) () noexcept<br> |
|  void | [**default\_model**](#function-default_model-12) (bool enable, const Json & config=default\_config()) noexcept<br> |
|  [**SubsceneModel**](classuipc_1_1core_1_1_subscene_model.md) | [**default\_model**](#function-default_model-22) () noexcept const<br> |
|  SizeT | [**element\_count**](#function-element_count) () noexcept const<br> |
|  IndexT | [**insert**](#function-insert) (const [**SubsceneElement**](classuipc_1_1core_1_1_subscene_element.md) & L, const [**SubsceneElement**](classuipc_1_1core_1_1_subscene_element.md) & R, bool enable=false, const Json & config=default\_config()) <br> |
|  [**SubsceneTabular**](classuipc_1_1core_1_1_subscene_tabular.md) & | [**operator=**](#function-operator) (const [**SubsceneTabular**](classuipc_1_1core_1_1_subscene_tabular.md) &) = delete<br> |
|  [**SubsceneModelCollection**](classuipc_1_1core_1_1_subscene_model_collection_t.md) | [**subscene\_models**](#function-subscene_models-12) () noexcept<br> |
|  [**CSubsceneModelCollection**](classuipc_1_1core_1_1_subscene_model_collection_t.md) | [**subscene\_models**](#function-subscene_models-22) () noexcept const<br> |
|   | [**~SubsceneTabular**](#function-subscenetabular) () noexcept<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Json | [**default\_config**](#function-default_config) () noexcept<br> |


























## Public Functions Documentation




### function SubsceneTabular [1/2]

```C++
uipc::core::SubsceneTabular::SubsceneTabular () noexcept
```




<hr>



### function SubsceneTabular [2/2]

```C++
uipc::core::SubsceneTabular::SubsceneTabular (
    const SubsceneTabular &
) = delete
```




<hr>



### function at 

```C++
SubsceneModel uipc::core::SubsceneTabular::at (
    SizeT i,
    SizeT j
) const
```




<hr>



### function create 

```C++
SubsceneElement uipc::core::SubsceneTabular::create (
    std::string_view name=""
) noexcept
```




<hr>



### function default\_element 

```C++
SubsceneElement uipc::core::SubsceneTabular::default_element () noexcept
```




<hr>



### function default\_model [1/2]

```C++
void uipc::core::SubsceneTabular::default_model (
    bool enable,
    const Json & config=default_config()
) noexcept
```




<hr>



### function default\_model [2/2]

```C++
SubsceneModel uipc::core::SubsceneTabular::default_model () noexcept const
```




<hr>



### function element\_count 

```C++
SizeT uipc::core::SubsceneTabular::element_count () noexcept const
```




<hr>



### function insert 

```C++
IndexT uipc::core::SubsceneTabular::insert (
    const SubsceneElement & L,
    const SubsceneElement & R,
    bool enable=false,
    const Json & config=default_config()
) 
```




<hr>



### function operator= 

```C++
SubsceneTabular & uipc::core::SubsceneTabular::operator= (
    const SubsceneTabular &
) = delete
```




<hr>



### function subscene\_models [1/2]

```C++
SubsceneModelCollection uipc::core::SubsceneTabular::subscene_models () noexcept
```




<hr>



### function subscene\_models [2/2]

```C++
CSubsceneModelCollection uipc::core::SubsceneTabular::subscene_models () noexcept const
```




<hr>



### function ~SubsceneTabular 

```C++
uipc::core::SubsceneTabular::~SubsceneTabular () noexcept
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::core::SubsceneTabular::default_config () noexcept
```




<hr>## Friends Documentation





### friend Scene 

```C++
class uipc::core::SubsceneTabular::Scene (
    internal::Scene
) 
```




<hr>



### friend to\_json 

```C++
UIPC_CORE_API void uipc::core::SubsceneTabular::to_json (
    Json & j,
    const SubsceneTabular & ct
) 
```




<hr>



### friend SubsceneTabularVisitor 

```C++
class uipc::core::SubsceneTabular::SubsceneTabularVisitor (
    uipc::backend::SubsceneTabularVisitor
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/subscene_tabular.h`

