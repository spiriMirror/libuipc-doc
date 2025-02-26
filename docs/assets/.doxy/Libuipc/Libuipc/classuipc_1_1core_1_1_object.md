

# Class uipc::core::Object



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**Object**](classuipc_1_1core_1_1_object.md)








Inherits the following classes: [uipc::core::IObject](classuipc_1_1core_1_1_i_object.md)












## Classes

| Type | Name |
| ---: | :--- |
| class | [**CGeometries**](classuipc_1_1core_1_1_object_1_1_c_geometries.md) <br> |
| class | [**Geometries**](classuipc_1_1core_1_1_object_1_1_geometries.md) <br> |










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Object**](#function-object-13) ([**Scene**](classuipc_1_1core_1_1_scene.md) & scene, IndexT id, std::string\_view name="") noexcept<br> |
|   | [**Object**](#function-object-23) ([**Object**](classuipc_1_1core_1_1_object.md) &&) = default<br> |
|   | [**Object**](#function-object-33) (const [**Object**](classuipc_1_1core_1_1_object.md) &) = delete<br> |
|  [**Geometries**](classuipc_1_1core_1_1_object_1_1_geometries.md) | [**geometries**](#function-geometries-12) () noexcept<br> |
|  [**CGeometries**](classuipc_1_1core_1_1_object_1_1_c_geometries.md) | [**geometries**](#function-geometries-22) () noexcept const<br> |
|  [**Object**](classuipc_1_1core_1_1_object.md) & | [**operator=**](#function-operator) (const [**Object**](classuipc_1_1core_1_1_object.md) &) = delete<br> |
|  [**Object**](classuipc_1_1core_1_1_object.md) & | [**operator=**](#function-operator_1) ([**Object**](classuipc_1_1core_1_1_object.md) &&) = delete<br> |
|   | [**~Object**](#function-object) () <br> |


## Public Functions inherited from uipc::core::IObject

See [uipc::core::IObject](classuipc_1_1core_1_1_i_object.md)

| Type | Name |
| ---: | :--- |
|  IndexT | [**id**](classuipc_1_1core_1_1_i_object.md#function-id) () noexcept const<br> |
|  std::string\_view | [**name**](classuipc_1_1core_1_1_i_object.md#function-name) () noexcept const<br> |
| virtual  | [**~IObject**](classuipc_1_1core_1_1_i_object.md#function-iobject) () = default<br> |














































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual IndexT | [**get\_id**](#function-get_id) () noexcept override const<br> |
| virtual std::string\_view | [**get\_name**](#function-get_name) () noexcept override const<br> |


## Protected Functions inherited from uipc::core::IObject

See [uipc::core::IObject](classuipc_1_1core_1_1_i_object.md)

| Type | Name |
| ---: | :--- |
| virtual IndexT | [**get\_id**](classuipc_1_1core_1_1_i_object.md#function-get_id) () noexcept const = 0<br> |
| virtual std::string\_view | [**get\_name**](classuipc_1_1core_1_1_i_object.md#function-get_name) () noexcept const = 0<br> |






## Public Functions Documentation




### function Object [1/3]

```C++
uipc::core::Object::Object (
    Scene & scene,
    IndexT id,
    std::string_view name=""
) noexcept
```




<hr>



### function Object [2/3]

```C++
uipc::core::Object::Object (
    Object &&
) = default
```




<hr>



### function Object [3/3]

```C++
uipc::core::Object::Object (
    const Object &
) = delete
```




<hr>



### function geometries [1/2]

```C++
Geometries uipc::core::Object::geometries () noexcept
```




<hr>



### function geometries [2/2]

```C++
CGeometries uipc::core::Object::geometries () noexcept const
```




<hr>



### function operator= 

```C++
Object & uipc::core::Object::operator= (
    const Object &
) = delete
```




<hr>



### function operator= 

```C++
Object & uipc::core::Object::operator= (
    Object &&
) = delete
```




<hr>



### function ~Object 

```C++
uipc::core::Object::~Object () 
```




<hr>
## Protected Functions Documentation




### function get\_id 

```C++
virtual IndexT uipc::core::Object::get_id () noexcept override const
```



Implements [*uipc::core::IObject::get\_id*](classuipc_1_1core_1_1_i_object.md#function-get_id)


<hr>



### function get\_name 

```C++
virtual std::string_view uipc::core::Object::get_name () noexcept override const
```



Implements [*uipc::core::IObject::get\_name*](classuipc_1_1core_1_1_i_object.md#function-get_name)


<hr>## Friends Documentation





### friend formatter&lt; Object &gt; 

```C++
struct uipc::core::Object::formatter< Object > (
    fmt::formatter< Object >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/object.h`

