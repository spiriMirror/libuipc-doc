

# Class uipc::geometry::GeometryCollection



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**GeometryCollection**](classuipc_1_1geometry_1_1_geometry_collection.md)








Inherits the following classes: [uipc::geometry::IGeometryCollection](classuipc_1_1geometry_1_1_i_geometry_collection.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GeometryCollection**](#function-geometrycollection-13) () = default<br> |
|   | [**GeometryCollection**](#function-geometrycollection-23) (const [**GeometryCollection**](classuipc_1_1geometry_1_1_geometry_collection.md) &) <br> |
|   | [**GeometryCollection**](#function-geometrycollection-33) ([**GeometryCollection**](classuipc_1_1geometry_1_1_geometry_collection.md) &&) noexcept<br> |
|  void | [**destroy**](#function-destroy) (IndexT id) noexcept<br> |
|  S&lt; [**geometry::GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md)&lt; GeometryT &gt; &gt; | [**emplace**](#function-emplace-12) (const GeometryT & geometry) <br> |
|  S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; | [**emplace**](#function-emplace-22) (const [**geometry::Geometry**](classuipc_1_1geometry_1_1_geometry.md) & geometry) <br> |
|  S&lt; [**geometry::GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md)&lt; GeometryT &gt; &gt; | [**find**](#function-find-14) (IndexT id) noexcept<br> |
|  S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; | [**find**](#function-find-24) (IndexT id) noexcept<br> |
|  S&lt; const [**geometry::GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md)&lt; GeometryT &gt; &gt; | [**find**](#function-find-34) (IndexT id) noexcept const<br> |
|  S&lt; const [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; | [**find**](#function-find-44) (IndexT id) noexcept const<br> |
|  span&lt; S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; &gt; | [**geometry\_slots**](#function-geometry_slots) () noexcept const<br> |
|  [**GeometryCollection**](classuipc_1_1geometry_1_1_geometry_collection.md) & | [**operator=**](#function-operator) (const [**GeometryCollection**](classuipc_1_1geometry_1_1_geometry_collection.md) &) = delete<br> |
|  [**GeometryCollection**](classuipc_1_1geometry_1_1_geometry_collection.md) & | [**operator=**](#function-operator_1) ([**GeometryCollection**](classuipc_1_1geometry_1_1_geometry_collection.md) &&) = default<br> |
|  span&lt; S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; &gt; | [**pending\_create\_slots**](#function-pending_create_slots) () noexcept const<br> |
|  void | [**pending\_destroy**](#function-pending_destroy) (IndexT id) noexcept<br> |
|  span&lt; IndexT &gt; | [**pending\_destroy\_ids**](#function-pending_destroy_ids) () noexcept const<br> |
|  S&lt; [**geometry::GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md)&lt; GeometryT &gt; &gt; | [**pending\_emplace**](#function-pending_emplace) (const GeometryT & geometry) <br> |
|  void | [**solve\_pending**](#function-solve_pending) () noexcept<br> |


## Public Functions inherited from uipc::geometry::IGeometryCollection

See [uipc::geometry::IGeometryCollection](classuipc_1_1geometry_1_1_i_geometry_collection.md)

| Type | Name |
| ---: | :--- |
|  void | [**clear**](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-clear) () noexcept<br> |
|  IndexT | [**next\_id**](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-next_id) () noexcept const<br> |
|  void | [**reserve**](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-reserve) (SizeT size) noexcept<br> |
|  SizeT | [**size**](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-size) () noexcept const<br> |
| virtual  | [**~IGeometryCollection**](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-igeometrycollection) () = default<br> |














































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_clear**](#function-do_clear) () noexcept override<br> |
| virtual void | [**do\_reserve**](#function-do_reserve) (SizeT size) noexcept override<br> |
| virtual IndexT | [**get\_next\_id**](#function-get_next_id) () noexcept override const<br> |
| virtual SizeT | [**get\_size**](#function-get_size) () noexcept override const<br> |


## Protected Functions inherited from uipc::geometry::IGeometryCollection

See [uipc::geometry::IGeometryCollection](classuipc_1_1geometry_1_1_i_geometry_collection.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_clear**](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-do_clear) () noexcept = 0<br> |
| virtual void | [**do\_reserve**](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-do_reserve) (SizeT size) noexcept = 0<br> |
| virtual IndexT | [**get\_next\_id**](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-get_next_id) () noexcept const = 0<br> |
| virtual SizeT | [**get\_size**](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-get_size) () noexcept const = 0<br> |






## Public Functions Documentation




### function GeometryCollection [1/3]

```C++
uipc::geometry::GeometryCollection::GeometryCollection () = default
```




<hr>



### function GeometryCollection [2/3]

```C++
uipc::geometry::GeometryCollection::GeometryCollection (
    const GeometryCollection &
) 
```




<hr>



### function GeometryCollection [3/3]

```C++
uipc::geometry::GeometryCollection::GeometryCollection (
    GeometryCollection &&
) noexcept
```




<hr>



### function destroy 

```C++
void uipc::geometry::GeometryCollection::destroy (
    IndexT id
) noexcept
```




<hr>



### function emplace [1/2]

```C++
template<std::derived_from< geometry::Geometry > GeometryT>
S< geometry::GeometrySlotT < GeometryT > > uipc::geometry::GeometryCollection::emplace (
    const GeometryT & geometry
) 
```




<hr>



### function emplace [2/2]

```C++
S< geometry::GeometrySlot > uipc::geometry::GeometryCollection::emplace (
    const geometry::Geometry & geometry
) 
```




<hr>



### function find [1/4]

```C++
template<std::derived_from< geometry::Geometry > GeometryT>
S< geometry::GeometrySlotT < GeometryT > > uipc::geometry::GeometryCollection::find (
    IndexT id
) noexcept
```




<hr>



### function find [2/4]

```C++
S< geometry::GeometrySlot > uipc::geometry::GeometryCollection::find (
    IndexT id
) noexcept
```




<hr>



### function find [3/4]

```C++
template<std::derived_from< geometry::Geometry > GeometryT>
S< const geometry::GeometrySlotT < GeometryT > > uipc::geometry::GeometryCollection::find (
    IndexT id
) noexcept const
```




<hr>



### function find [4/4]

```C++
S< const geometry::GeometrySlot > uipc::geometry::GeometryCollection::find (
    IndexT id
) noexcept const
```




<hr>



### function geometry\_slots 

```C++
span< S< geometry::GeometrySlot > > uipc::geometry::GeometryCollection::geometry_slots () noexcept const
```




<hr>



### function operator= 

```C++
GeometryCollection & uipc::geometry::GeometryCollection::operator= (
    const GeometryCollection &
) = delete
```




<hr>



### function operator= 

```C++
GeometryCollection & uipc::geometry::GeometryCollection::operator= (
    GeometryCollection &&
) = default
```




<hr>



### function pending\_create\_slots 

```C++
span< S< geometry::GeometrySlot > > uipc::geometry::GeometryCollection::pending_create_slots () noexcept const
```




<hr>



### function pending\_destroy 

```C++
void uipc::geometry::GeometryCollection::pending_destroy (
    IndexT id
) noexcept
```




<hr>



### function pending\_destroy\_ids 

```C++
span< IndexT > uipc::geometry::GeometryCollection::pending_destroy_ids () noexcept const
```




<hr>



### function pending\_emplace 

```C++
template<std::derived_from< geometry::Geometry > GeometryT>
S< geometry::GeometrySlotT < GeometryT > > uipc::geometry::GeometryCollection::pending_emplace (
    const GeometryT & geometry
) 
```




<hr>



### function solve\_pending 

```C++
void uipc::geometry::GeometryCollection::solve_pending () noexcept
```




<hr>
## Protected Functions Documentation




### function do\_clear 

```C++
virtual void uipc::geometry::GeometryCollection::do_clear () noexcept override
```



Implements [*uipc::geometry::IGeometryCollection::do\_clear*](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-do_clear)


<hr>



### function do\_reserve 

```C++
virtual void uipc::geometry::GeometryCollection::do_reserve (
    SizeT size
) noexcept override
```



Implements [*uipc::geometry::IGeometryCollection::do\_reserve*](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-do_reserve)


<hr>



### function get\_next\_id 

```C++
virtual IndexT uipc::geometry::GeometryCollection::get_next_id () noexcept override const
```



Implements [*uipc::geometry::IGeometryCollection::get\_next\_id*](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-get_next_id)


<hr>



### function get\_size 

```C++
virtual SizeT uipc::geometry::GeometryCollection::get_size () noexcept override const
```



Implements [*uipc::geometry::IGeometryCollection::get\_size*](classuipc_1_1geometry_1_1_i_geometry_collection.md#function-get_size)


<hr>## Friends Documentation





### friend SceneFactory 

```C++
class uipc::geometry::GeometryCollection::SceneFactory (
    core::SceneFactory
) 
```




<hr>



### friend Scene 

```C++
class uipc::geometry::GeometryCollection::Scene (
    core::internal::Scene
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry_collection.h`

