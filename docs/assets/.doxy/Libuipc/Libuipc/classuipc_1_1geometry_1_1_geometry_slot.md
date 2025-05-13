

# Class uipc::geometry::GeometrySlot



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md)










Inherited by the following classes: [uipc::geometry::GeometrySlotT&lt; Geometry &gt;](classuipc_1_1geometry_1_1_geometry_slot_t_3_01_geometry_01_4.md),  [uipc::geometry::GeometrySlotT&lt; ImplicitGeometry &gt;](classuipc_1_1geometry_1_1_geometry_slot_t_3_01_implicit_geometry_01_4.md),  [uipc::geometry::GeometrySlotT&lt; SimplicialComplex &gt;](classuipc_1_1geometry_1_1_geometry_slot_t_3_01_simplicial_complex_01_4.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GeometrySlot**](#function-geometryslot-13) (IndexT id) noexcept<br> |
|   | [**GeometrySlot**](#function-geometryslot-23) (const [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &) = delete<br> |
|   | [**GeometrySlot**](#function-geometryslot-33) ([**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &&) = delete<br> |
|  S&lt; [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; | [**clone**](#function-clone) () const<br> |
|  [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**geometry**](#function-geometry-12) () noexcept<br> |
|  const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**geometry**](#function-geometry-22) () noexcept const<br> |
|  IndexT | [**id**](#function-id-12) () noexcept const<br> |
|  [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) & | [**operator=**](#function-operator) (const [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &) = delete<br> |
|  [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) & | [**operator=**](#function-operator_1) ([**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &&) = delete<br> |
|  GeometrySlotState | [**state**](#function-state-12) () noexcept const<br> |
| virtual  | [**~GeometrySlot**](#function-geometryslot) () = default<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual S&lt; [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &gt; | [**do\_clone**](#function-do_clone) () const = 0<br> |
| virtual [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**get\_geometry**](#function-get_geometry-12) () noexcept = 0<br> |
| virtual const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**get\_geometry**](#function-get_geometry-22) () noexcept const = 0<br> |




## Public Functions Documentation




### function GeometrySlot [1/3]

```C++
uipc::geometry::GeometrySlot::GeometrySlot (
    IndexT id
) noexcept
```




<hr>



### function GeometrySlot [2/3]

```C++
uipc::geometry::GeometrySlot::GeometrySlot (
    const GeometrySlot &
) = delete
```




<hr>



### function GeometrySlot [3/3]

```C++
uipc::geometry::GeometrySlot::GeometrySlot (
    GeometrySlot &&
) = delete
```




<hr>



### function clone 

```C++
S< GeometrySlot > uipc::geometry::GeometrySlot::clone () const
```




<hr>



### function geometry [1/2]

```C++
Geometry & uipc::geometry::GeometrySlot::geometry () noexcept
```




<hr>



### function geometry [2/2]

```C++
const Geometry & uipc::geometry::GeometrySlot::geometry () noexcept const
```




<hr>



### function id [1/2]

```C++
IndexT uipc::geometry::GeometrySlot::id () noexcept const
```




<hr>



### function operator= 

```C++
GeometrySlot & uipc::geometry::GeometrySlot::operator= (
    const GeometrySlot &
) = delete
```




<hr>



### function operator= 

```C++
GeometrySlot & uipc::geometry::GeometrySlot::operator= (
    GeometrySlot &&
) = delete
```




<hr>



### function state [1/2]

```C++
GeometrySlotState uipc::geometry::GeometrySlot::state () noexcept const
```




<hr>



### function ~GeometrySlot 

```C++
virtual uipc::geometry::GeometrySlot::~GeometrySlot () = default
```




<hr>
## Protected Functions Documentation




### function do\_clone 

```C++
virtual S< GeometrySlot > uipc::geometry::GeometrySlot::do_clone () const = 0
```




<hr>



### function get\_geometry [1/2]

```C++
virtual Geometry & uipc::geometry::GeometrySlot::get_geometry () noexcept = 0
```




<hr>



### function get\_geometry [2/2]

```C++
virtual const Geometry & uipc::geometry::GeometrySlot::get_geometry () noexcept const = 0
```




<hr>## Friends Documentation





### friend SceneFactory 

```C++
class uipc::geometry::GeometrySlot::SceneFactory (
    core::SceneFactory
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry_slot.h`

