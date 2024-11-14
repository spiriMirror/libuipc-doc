

# Class uipc::geometry::GeometrySlotT&lt; SimplicialComplex &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**GeometrySlotT&lt; SimplicialComplex &gt;**](classuipc_1_1geometry_1_1_geometry_slot_t_3_01_simplicial_complex_01_4.md)








Inherits the following classes: [uipc::geometry::GeometrySlot](classuipc_1_1geometry_1_1_geometry_slot.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GeometrySlotT**](#function-geometryslott-13) (IndexT id, const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & simplicial\_complex) noexcept<br> |
|   | [**GeometrySlotT**](#function-geometryslott-23) (const [**GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md) &) = delete<br> |
|   | [**GeometrySlotT**](#function-geometryslott-33) ([**GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md) &&) = delete<br> |
|  [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & | [**geometry**](#function-geometry-12) () noexcept<br> |
|  const [**SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & | [**geometry**](#function-geometry-22) () noexcept const<br> |
|  [**GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md) & | [**operator=**](#function-operator) (const [**GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md) &) = delete<br> |
|  [**GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md) & | [**operator=**](#function-operator_1) ([**GeometrySlotT**](classuipc_1_1geometry_1_1_geometry_slot_t.md) &&) = delete<br> |


## Public Functions inherited from uipc::geometry::GeometrySlot

See [uipc::geometry::GeometrySlot](classuipc_1_1geometry_1_1_geometry_slot.md)

| Type | Name |
| ---: | :--- |
|   | [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md#function-geometryslot-13) (IndexT id) noexcept<br> |
|   | [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md#function-geometryslot-23) (const [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &) = delete<br> |
|   | [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md#function-geometryslot-33) ([**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &&) = delete<br> |
|  [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**geometry**](classuipc_1_1geometry_1_1_geometry_slot.md#function-geometry-12) () noexcept<br> |
|  const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**geometry**](classuipc_1_1geometry_1_1_geometry_slot.md#function-geometry-22) () noexcept const<br> |
|  IndexT | [**id**](classuipc_1_1geometry_1_1_geometry_slot.md#function-id) () noexcept const<br> |
|  [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) & | [**operator=**](classuipc_1_1geometry_1_1_geometry_slot.md#function-operator) (const [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &) = delete<br> |
|  [**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) & | [**operator=**](classuipc_1_1geometry_1_1_geometry_slot.md#function-operator_1) ([**GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md) &&) = delete<br> |
|  GeometrySlotState | [**state**](classuipc_1_1geometry_1_1_geometry_slot.md#function-state-12) () noexcept const<br> |
| virtual  | [**~GeometrySlot**](classuipc_1_1geometry_1_1_geometry_slot.md#function-geometryslot) () = default<br> |














































## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**get\_geometry**](#function-get_geometry-12) () noexcept override<br> |
| virtual const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**get\_geometry**](#function-get_geometry-22) () noexcept override const<br> |


## Protected Functions inherited from uipc::geometry::GeometrySlot

See [uipc::geometry::GeometrySlot](classuipc_1_1geometry_1_1_geometry_slot.md)

| Type | Name |
| ---: | :--- |
| virtual [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**get\_geometry**](classuipc_1_1geometry_1_1_geometry_slot.md#function-get_geometry-12) () noexcept = 0<br> |
| virtual const [**Geometry**](classuipc_1_1geometry_1_1_geometry.md) & | [**get\_geometry**](classuipc_1_1geometry_1_1_geometry_slot.md#function-get_geometry-22) () noexcept const = 0<br> |






## Public Functions Documentation




### function GeometrySlotT [1/3]

```C++
uipc::geometry::GeometrySlotT< SimplicialComplex >::GeometrySlotT (
    IndexT id,
    const SimplicialComplex & simplicial_complex
) noexcept
```




<hr>



### function GeometrySlotT [2/3]

```C++
uipc::geometry::GeometrySlotT< SimplicialComplex >::GeometrySlotT (
    const GeometrySlotT &
) = delete
```




<hr>



### function GeometrySlotT [3/3]

```C++
uipc::geometry::GeometrySlotT< SimplicialComplex >::GeometrySlotT (
    GeometrySlotT &&
) = delete
```




<hr>



### function geometry [1/2]

```C++
SimplicialComplex & uipc::geometry::GeometrySlotT< SimplicialComplex >::geometry () noexcept
```




<hr>



### function geometry [2/2]

```C++
const SimplicialComplex & uipc::geometry::GeometrySlotT< SimplicialComplex >::geometry () noexcept const
```




<hr>



### function operator= 

```C++
GeometrySlotT & uipc::geometry::GeometrySlotT< SimplicialComplex >::operator= (
    const GeometrySlotT &
) = delete
```




<hr>



### function operator= 

```C++
GeometrySlotT & uipc::geometry::GeometrySlotT< SimplicialComplex >::operator= (
    GeometrySlotT &&
) = delete
```




<hr>
## Protected Functions Documentation




### function get\_geometry [1/2]

```C++
virtual Geometry & uipc::geometry::GeometrySlotT< SimplicialComplex >::get_geometry () noexcept override
```



Implements [*uipc::geometry::GeometrySlot::get\_geometry*](classuipc_1_1geometry_1_1_geometry_slot.md#function-get_geometry-12)


<hr>



### function get\_geometry [2/2]

```C++
virtual const Geometry & uipc::geometry::GeometrySlotT< SimplicialComplex >::get_geometry () noexcept override const
```



Implements [*uipc::geometry::GeometrySlot::get\_geometry*](classuipc_1_1geometry_1_1_geometry_slot.md#function-get_geometry-22)


<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/simplicial_complex_slot.h`

