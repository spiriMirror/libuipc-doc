

# Class uipc::core::Scene::Objects



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**Scene**](classuipc_1_1core_1_1_scene.md) **>** [**Objects**](classuipc_1_1core_1_1_scene_1_1_objects.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  S&lt; [**Object**](classuipc_1_1core_1_1_object.md) &gt; | [**create**](#function-create) (std::string\_view name="") <br> |
|  SizeT | [**created\_count**](#function-created_count) () noexcept const<br> |
|  void | [**destroy**](#function-destroy) (IndexT id) <br> |
|  S&lt; [**Object**](classuipc_1_1core_1_1_object.md) &gt; | [**find**](#function-find-12) (IndexT id) noexcept<br> |
|  vector&lt; S&lt; [**Object**](classuipc_1_1core_1_1_object.md) &gt; &gt; | [**find**](#function-find-22) (std::string\_view name) noexcept<br> |
|  SizeT | [**size**](#function-size) () noexcept const<br> |




























## Public Functions Documentation




### function create 

```C++
S< Object > uipc::core::Scene::Objects::create (
    std::string_view name=""
) 
```




<hr>



### function created\_count 

```C++
SizeT uipc::core::Scene::Objects::created_count () noexcept const
```




<hr>



### function destroy 

```C++
void uipc::core::Scene::Objects::destroy (
    IndexT id
) 
```




<hr>



### function find [1/2]

```C++
S< Object > uipc::core::Scene::Objects::find (
    IndexT id
) noexcept
```




<hr>



### function find [2/2]

```C++
vector< S< Object > > uipc::core::Scene::Objects::find (
    std::string_view name
) noexcept
```




<hr>



### function size 

```C++
SizeT uipc::core::Scene::Objects::size () noexcept const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/scene.h`

