

# Class uipc::core::SubsceneElement



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SubsceneElement**](classuipc_1_1core_1_1_subscene_element.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SubsceneElement**](#function-subsceneelement-14) () = default<br> |
|   | [**SubsceneElement**](#function-subsceneelement-24) (const [**SubsceneElement**](classuipc_1_1core_1_1_subscene_element.md) &) = default<br> |
|   | [**SubsceneElement**](#function-subsceneelement-34) ([**SubsceneElement**](classuipc_1_1core_1_1_subscene_element.md) &&) = default<br> |
|   | [**SubsceneElement**](#function-subsceneelement-44) (IndexT id, std::string\_view name) noexcept<br> |
|  S&lt; [**geometry::AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; IndexT &gt; &gt; | [**apply\_to**](#function-apply_to) ([**geometry::Geometry**](classuipc_1_1geometry_1_1_geometry.md) & geo) const<br> |
|  IndexT | [**id**](#function-id) () noexcept const<br> |
|  std::string\_view | [**name**](#function-name) () noexcept const<br> |
|  [**SubsceneElement**](classuipc_1_1core_1_1_subscene_element.md) & | [**operator=**](#function-operator) (const [**SubsceneElement**](classuipc_1_1core_1_1_subscene_element.md) &) = default<br> |
|  [**SubsceneElement**](classuipc_1_1core_1_1_subscene_element.md) & | [**operator=**](#function-operator_1) ([**SubsceneElement**](classuipc_1_1core_1_1_subscene_element.md) &&) = default<br> |




























## Public Functions Documentation




### function SubsceneElement [1/4]

```C++
uipc::core::SubsceneElement::SubsceneElement () = default
```




<hr>



### function SubsceneElement [2/4]

```C++
uipc::core::SubsceneElement::SubsceneElement (
    const SubsceneElement &
) = default
```




<hr>



### function SubsceneElement [3/4]

```C++
uipc::core::SubsceneElement::SubsceneElement (
    SubsceneElement &&
) = default
```




<hr>



### function SubsceneElement [4/4]

```C++
uipc::core::SubsceneElement::SubsceneElement (
    IndexT id,
    std::string_view name
) noexcept
```




<hr>



### function apply\_to 

```C++
S< geometry::AttributeSlot < IndexT > > uipc::core::SubsceneElement::apply_to (
    geometry::Geometry & geo
) const
```




<hr>



### function id 

```C++
IndexT uipc::core::SubsceneElement::id () noexcept const
```




<hr>



### function name 

```C++
std::string_view uipc::core::SubsceneElement::name () noexcept const
```




<hr>



### function operator= 

```C++
SubsceneElement & uipc::core::SubsceneElement::operator= (
    const SubsceneElement &
) = default
```




<hr>



### function operator= 

```C++
SubsceneElement & uipc::core::SubsceneElement::operator= (
    SubsceneElement &&
) = default
```




<hr>## Friends Documentation





### friend from\_json 

```C++
UIPC_CORE_API void uipc::core::SubsceneElement::from_json (
    const Json & j,
    SubsceneElement & element
) 
```




<hr>



### friend to\_json 

```C++
UIPC_CORE_API void uipc::core::SubsceneElement::to_json (
    Json & j,
    const SubsceneElement & element
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/subscene_element.h`

