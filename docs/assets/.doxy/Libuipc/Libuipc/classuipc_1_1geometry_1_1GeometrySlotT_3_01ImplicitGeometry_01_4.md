

# Class uipc::geometry::GeometrySlotT&lt; ImplicitGeometry &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**GeometrySlotT&lt; ImplicitGeometry &gt;**](classuipc_1_1geometry_1_1GeometrySlotT_3_01ImplicitGeometry_01_4.md)








Inherits the following classes: [uipc::geometry::GeometrySlot](classuipc_1_1geometry_1_1GeometrySlot.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GeometrySlotT**](#function-geometryslott) (IndexT id, const [**ImplicitGeometry**](classuipc_1_1geometry_1_1ImplicitGeometry.md) & geometry) <br> |
|  [**ImplicitGeometry**](classuipc_1_1geometry_1_1ImplicitGeometry.md) & | [**geometry**](#function-geometry-12) () noexcept<br> |
|  const [**ImplicitGeometry**](classuipc_1_1geometry_1_1ImplicitGeometry.md) & | [**geometry**](#function-geometry-22) () noexcept const<br> |


## Public Functions inherited from uipc::geometry::GeometrySlot

See [uipc::geometry::GeometrySlot](classuipc_1_1geometry_1_1GeometrySlot.md)

| Type | Name |
| ---: | :--- |
|   | [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md#function-geometryslot-13) (IndexT id) noexcept<br> |
|   | [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md#function-geometryslot-23) (const [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &) = delete<br> |
|   | [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md#function-geometryslot-33) ([**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &&) = delete<br> |
|  S&lt; [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &gt; | [**clone**](classuipc_1_1geometry_1_1GeometrySlot.md#function-clone) () const<br> |
|  [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & | [**geometry**](classuipc_1_1geometry_1_1GeometrySlot.md#function-geometry-12) () noexcept<br> |
|  const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & | [**geometry**](classuipc_1_1geometry_1_1GeometrySlot.md#function-geometry-22) () noexcept const<br> |
|  IndexT | [**id**](classuipc_1_1geometry_1_1GeometrySlot.md#function-id-12) () noexcept const<br> |
|  [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) & | [**operator=**](classuipc_1_1geometry_1_1GeometrySlot.md#function-operator) (const [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &) = delete<br> |
|  [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) & | [**operator=**](classuipc_1_1geometry_1_1GeometrySlot.md#function-operator_1) ([**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &&) = delete<br> |
|  GeometrySlotState | [**state**](classuipc_1_1geometry_1_1GeometrySlot.md#function-state-12) () noexcept const<br> |
| virtual  | [**~GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md#function-geometryslot) () = default<br> |














































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual S&lt; [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &gt; | [**do\_clone**](#function-do_clone) () override const<br> |
| virtual [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & | [**get\_geometry**](#function-get_geometry-12) () noexcept override<br> |
| virtual const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & | [**get\_geometry**](#function-get_geometry-22) () noexcept override const<br> |


## Protected Functions inherited from uipc::geometry::GeometrySlot

See [uipc::geometry::GeometrySlot](classuipc_1_1geometry_1_1GeometrySlot.md)

| Type | Name |
| ---: | :--- |
| virtual S&lt; [**GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &gt; | [**do\_clone**](classuipc_1_1geometry_1_1GeometrySlot.md#function-do_clone) () const = 0<br> |
| virtual [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & | [**get\_geometry**](classuipc_1_1geometry_1_1GeometrySlot.md#function-get_geometry-12) () noexcept = 0<br> |
| virtual const [**Geometry**](classuipc_1_1geometry_1_1Geometry.md) & | [**get\_geometry**](classuipc_1_1geometry_1_1GeometrySlot.md#function-get_geometry-22) () noexcept const = 0<br> |






## Public Functions Documentation




### function GeometrySlotT 

```C++
uipc::geometry::GeometrySlotT< ImplicitGeometry >::GeometrySlotT (
    IndexT id,
    const ImplicitGeometry & geometry
) 
```




<hr>



### function geometry [1/2]

```C++
ImplicitGeometry & uipc::geometry::GeometrySlotT< ImplicitGeometry >::geometry () noexcept
```




<hr>



### function geometry [2/2]

```C++
const ImplicitGeometry & uipc::geometry::GeometrySlotT< ImplicitGeometry >::geometry () noexcept const
```




<hr>
## Protected Functions Documentation




### function do\_clone 

```C++
virtual S< GeometrySlot > uipc::geometry::GeometrySlotT< ImplicitGeometry >::do_clone () override const
```



Implements [*uipc::geometry::GeometrySlot::do\_clone*](classuipc_1_1geometry_1_1GeometrySlot.md#function-do_clone)


<hr>



### function get\_geometry [1/2]

```C++
virtual Geometry & uipc::geometry::GeometrySlotT< ImplicitGeometry >::get_geometry () noexcept override
```



Implements [*uipc::geometry::GeometrySlot::get\_geometry*](classuipc_1_1geometry_1_1GeometrySlot.md#function-get_geometry-12)


<hr>



### function get\_geometry [2/2]

```C++
virtual const Geometry & uipc::geometry::GeometrySlotT< ImplicitGeometry >::get_geometry () noexcept override const
```



Implements [*uipc::geometry::GeometrySlot::get\_geometry*](classuipc_1_1geometry_1_1GeometrySlot.md#function-get_geometry-22)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/implicit_geometry_slot.h`

