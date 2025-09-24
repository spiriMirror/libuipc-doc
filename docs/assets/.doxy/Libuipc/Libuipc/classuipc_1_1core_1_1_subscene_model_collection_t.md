

# Class uipc::core::SubsceneModelCollectionT

**template &lt;bool IsConst&gt;**



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**SubsceneModelCollectionT**](classuipc_1_1core_1_1_subscene_model_collection_t.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  auto | [**create**](#function-create) (std::string\_view name, const T & default\_value={}, bool allow\_destroy=true) <br> |
|  auto | [**find**](#function-find-12) (std::string\_view name) <br> |
|  auto | [**find**](#function-find-22) (std::string\_view name) <br> |
|  auto | [**to\_json**](#function-to_json) () const<br> |




























## Public Functions Documentation




### function create 

```C++
template<typename T>
inline auto uipc::core::SubsceneModelCollectionT::create (
    std::string_view name,
    const T & default_value={},
    bool allow_destroy=true
) 
```




<hr>



### function find [1/2]

```C++
template<typename T>
inline auto uipc::core::SubsceneModelCollectionT::find (
    std::string_view name
) 
```




<hr>



### function find [2/2]

```C++
inline auto uipc::core::SubsceneModelCollectionT::find (
    std::string_view name
) 
```




<hr>



### function to\_json 

```C++
inline auto uipc::core::SubsceneModelCollectionT::to_json () const
```




<hr>## Friends Documentation





### friend AttributeFriend 

```C++
template<typename T>
class uipc::core::SubsceneModelCollectionT::AttributeFriend (
    geometry::AttributeFriend
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/subscene_model_collection.h`

