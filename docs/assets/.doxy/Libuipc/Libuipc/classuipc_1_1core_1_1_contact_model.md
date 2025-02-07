

# Class uipc::core::ContactModel



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ContactModel**](classuipc_1_1core_1_1_contact_model.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ContactModel**](#function-contactmodel-12) () noexcept<br> |
|   | [**ContactModel**](#function-contactmodel-22) (const Vector2i & ids, Float friction\_rate, Float resistance, bool enable, const Json & config) <br> |
|  const Json & | [**config**](#function-config) () const<br> |
|  Float | [**friction\_rate**](#function-friction_rate) () const<br> |
|  bool | [**is\_enabled**](#function-is_enabled) () const<br> |
|  Float | [**resistance**](#function-resistance) () const<br> |
|  const Vector2i & | [**topo**](#function-topo) () const<br> |




























## Public Functions Documentation




### function ContactModel [1/2]

```C++
uipc::core::ContactModel::ContactModel () noexcept
```




<hr>



### function ContactModel [2/2]

```C++
uipc::core::ContactModel::ContactModel (
    const Vector2i & ids,
    Float friction_rate,
    Float resistance,
    bool enable,
    const Json & config
) 
```




<hr>



### function config 

```C++
const Json & uipc::core::ContactModel::config () const
```




<hr>



### function friction\_rate 

```C++
Float uipc::core::ContactModel::friction_rate () const
```




<hr>



### function is\_enabled 

```C++
bool uipc::core::ContactModel::is_enabled () const
```




<hr>



### function resistance 

```C++
Float uipc::core::ContactModel::resistance () const
```




<hr>



### function topo 

```C++
const Vector2i & uipc::core::ContactModel::topo () const
```




<hr>## Friends Documentation





### friend from\_json 

```C++
void uipc::core::ContactModel::from_json (
    const Json & json,
    ContactModel & model
) 
```




<hr>



### friend to\_json 

```C++
void uipc::core::ContactModel::to_json (
    Json & json,
    const ContactModel & model
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/contact_model.h`

