

# Class uipc::core::ContactElement



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ContactElement**](classuipc_1_1core_1_1_contact_element.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ContactElement**](#function-contactelement-14) () = default<br> |
|   | [**ContactElement**](#function-contactelement-24) (const [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) &) = default<br> |
|   | [**ContactElement**](#function-contactelement-34) ([**ContactElement**](classuipc_1_1core_1_1_contact_element.md) &&) = default<br> |
|   | [**ContactElement**](#function-contactelement-44) (IndexT id, std::string\_view name) noexcept<br> |
|  S&lt; [**geometry::AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; IndexT &gt; &gt; | [**apply\_to**](#function-apply_to) ([**geometry::Geometry**](classuipc_1_1geometry_1_1_geometry.md) & geo) const<br> |
|  IndexT | [**id**](#function-id) () noexcept const<br> |
|  std::string\_view | [**name**](#function-name) () noexcept const<br> |
|  [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & | [**operator=**](#function-operator) (const [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) &) = default<br> |
|  [**ContactElement**](classuipc_1_1core_1_1_contact_element.md) & | [**operator=**](#function-operator_1) ([**ContactElement**](classuipc_1_1core_1_1_contact_element.md) &&) = default<br> |




























## Public Functions Documentation




### function ContactElement [1/4]

```C++
uipc::core::ContactElement::ContactElement () = default
```




<hr>



### function ContactElement [2/4]

```C++
uipc::core::ContactElement::ContactElement (
    const ContactElement &
) = default
```




<hr>



### function ContactElement [3/4]

```C++
uipc::core::ContactElement::ContactElement (
    ContactElement &&
) = default
```




<hr>



### function ContactElement [4/4]

```C++
uipc::core::ContactElement::ContactElement (
    IndexT id,
    std::string_view name
) noexcept
```




<hr>



### function apply\_to 

```C++
S< geometry::AttributeSlot < IndexT > > uipc::core::ContactElement::apply_to (
    geometry::Geometry & geo
) const
```




<hr>



### function id 

```C++
IndexT uipc::core::ContactElement::id () noexcept const
```




<hr>



### function name 

```C++
std::string_view uipc::core::ContactElement::name () noexcept const
```




<hr>



### function operator= 

```C++
ContactElement & uipc::core::ContactElement::operator= (
    const ContactElement &
) = default
```




<hr>



### function operator= 

```C++
ContactElement & uipc::core::ContactElement::operator= (
    ContactElement &&
) = default
```




<hr>## Friends Documentation





### friend from\_json 

```C++
void uipc::core::ContactElement::from_json (
    const Json & j,
    ContactElement & element
) 
```




<hr>



### friend to\_json 

```C++
void uipc::core::ContactElement::to_json (
    Json & j,
    const ContactElement & element
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/contact_element.h`

