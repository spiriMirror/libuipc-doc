

# Class uipc::core::ObjectCollection



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ObjectCollection**](classuipc_1_1core_1_1ObjectCollection.md)








Inherits the following classes: [uipc::core::IObjectCollection](classuipc_1_1core_1_1IObjectCollection.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ObjectCollection**](#function-objectcollection) () = default<br> |
|  void | [**destroy**](#function-destroy) (IndexT id) noexcept<br> |
|  S&lt; [**Object**](classuipc_1_1core_1_1Object.md) &gt; | [**emplace**](#function-emplace) ([**Object**](classuipc_1_1core_1_1Object.md) && object) <br> |
|  S&lt; [**Object**](classuipc_1_1core_1_1Object.md) &gt; | [**find**](#function-find-14) (IndexT id) noexcept<br> |
|  S&lt; const [**Object**](classuipc_1_1core_1_1Object.md) &gt; | [**find**](#function-find-24) (IndexT id) noexcept const<br> |
|  vector&lt; S&lt; [**Object**](classuipc_1_1core_1_1Object.md) &gt; &gt; | [**find**](#function-find-34) (std::string\_view name) noexcept<br> |
|  vector&lt; S&lt; const [**Object**](classuipc_1_1core_1_1Object.md) &gt; &gt; | [**find**](#function-find-44) (std::string\_view name) noexcept const<br> |
|  IndexT | [**next\_id**](#function-next_id) () noexcept const<br> |
|  void | [**reserve**](#function-reserve) (SizeT size) noexcept<br> |
|  SizeT | [**size**](#function-size) () noexcept const<br> |


## Public Functions inherited from uipc::core::IObjectCollection

See [uipc::core::IObjectCollection](classuipc_1_1core_1_1IObjectCollection.md)

| Type | Name |
| ---: | :--- |
| virtual  | [**~IObjectCollection**](classuipc_1_1core_1_1IObjectCollection.md#function-iobjectcollection) () = default<br> |






















































## Public Functions Documentation




### function ObjectCollection 

```C++
uipc::core::ObjectCollection::ObjectCollection () = default
```




<hr>



### function destroy 

```C++
void uipc::core::ObjectCollection::destroy (
    IndexT id
) noexcept
```




<hr>



### function emplace 

```C++
S< Object > uipc::core::ObjectCollection::emplace (
    Object && object
) 
```




<hr>



### function find [1/4]

```C++
S< Object > uipc::core::ObjectCollection::find (
    IndexT id
) noexcept
```




<hr>



### function find [2/4]

```C++
S< const Object > uipc::core::ObjectCollection::find (
    IndexT id
) noexcept const
```




<hr>



### function find [3/4]

```C++
vector< S< Object > > uipc::core::ObjectCollection::find (
    std::string_view name
) noexcept
```




<hr>



### function find [4/4]

```C++
vector< S< const Object > > uipc::core::ObjectCollection::find (
    std::string_view name
) noexcept const
```




<hr>



### function next\_id 

```C++
IndexT uipc::core::ObjectCollection::next_id () noexcept const
```




<hr>



### function reserve 

```C++
void uipc::core::ObjectCollection::reserve (
    SizeT size
) noexcept
```




<hr>



### function size 

```C++
SizeT uipc::core::ObjectCollection::size () noexcept const
```




<hr>## Friends Documentation





### friend formatter&lt; ObjectCollection &gt; 

```C++
struct uipc::core::ObjectCollection::formatter< ObjectCollection > (
    fmt::formatter< ObjectCollection >
) 
```




<hr>



### friend Scene 

```C++
class uipc::core::ObjectCollection::Scene (
    internal::Scene
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/object_collection.h`

