

# Class uipc::core::SubsceneModel



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SubsceneModel**](classuipc_1_1core_1_1_subscene_model.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SubsceneModel**](#function-subscenemodel-12) () noexcept<br> |
|   | [**SubsceneModel**](#function-subscenemodel-22) (const Vector2i & ids, bool enable, const Json & config) <br> |
|  const Json & | [**config**](#function-config) () const<br> |
|  bool | [**is\_enabled**](#function-is_enabled) () const<br> |
|  const Vector2i & | [**topo**](#function-topo) () const<br> |




























## Public Functions Documentation




### function SubsceneModel [1/2]

```C++
uipc::core::SubsceneModel::SubsceneModel () noexcept
```




<hr>



### function SubsceneModel [2/2]

```C++
uipc::core::SubsceneModel::SubsceneModel (
    const Vector2i & ids,
    bool enable,
    const Json & config
) 
```




<hr>



### function config 

```C++
const Json & uipc::core::SubsceneModel::config () const
```




<hr>



### function is\_enabled 

```C++
bool uipc::core::SubsceneModel::is_enabled () const
```




<hr>



### function topo 

```C++
const Vector2i & uipc::core::SubsceneModel::topo () const
```




<hr>## Friends Documentation





### friend from\_json 

```C++
void uipc::core::SubsceneModel::from_json (
    const Json & json,
    SubsceneModel & model
) 
```




<hr>



### friend to\_json 

```C++
void uipc::core::SubsceneModel::to_json (
    Json & json,
    const SubsceneModel & model
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/subscene_model.h`

