

# Class uipc::geometry::IGeometryCollection



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**IGeometryCollection**](classuipc_1_1geometry_1_1IGeometryCollection.md)










Inherited by the following classes: [uipc::geometry::GeometryCollection](classuipc_1_1geometry_1_1GeometryCollection.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**clear**](#function-clear) () noexcept<br> |
|  IndexT | [**next\_id**](#function-next_id) () noexcept const<br> |
|  void | [**reserve**](#function-reserve) (SizeT size) noexcept<br> |
|  SizeT | [**size**](#function-size) () noexcept const<br> |
| virtual  | [**~IGeometryCollection**](#function-igeometrycollection) () = default<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_clear**](#function-do_clear) () noexcept = 0<br> |
| virtual void | [**do\_reserve**](#function-do_reserve) (SizeT size) noexcept = 0<br> |
| virtual IndexT | [**get\_next\_id**](#function-get_next_id) () noexcept const = 0<br> |
| virtual SizeT | [**get\_size**](#function-get_size) () noexcept const = 0<br> |




## Public Functions Documentation




### function clear 

```C++
void uipc::geometry::IGeometryCollection::clear () noexcept
```




<hr>



### function next\_id 

```C++
IndexT uipc::geometry::IGeometryCollection::next_id () noexcept const
```




<hr>



### function reserve 

```C++
void uipc::geometry::IGeometryCollection::reserve (
    SizeT size
) noexcept
```




<hr>



### function size 

```C++
SizeT uipc::geometry::IGeometryCollection::size () noexcept const
```




<hr>



### function ~IGeometryCollection 

```C++
virtual uipc::geometry::IGeometryCollection::~IGeometryCollection () = default
```




<hr>
## Protected Functions Documentation




### function do\_clear 

```C++
virtual void uipc::geometry::IGeometryCollection::do_clear () noexcept = 0
```




<hr>



### function do\_reserve 

```C++
virtual void uipc::geometry::IGeometryCollection::do_reserve (
    SizeT size
) noexcept = 0
```




<hr>



### function get\_next\_id 

```C++
virtual IndexT uipc::geometry::IGeometryCollection::get_next_id () noexcept const = 0
```




<hr>



### function get\_size 

```C++
virtual SizeT uipc::geometry::IGeometryCollection::get_size () noexcept const = 0
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/geometry_collection.h`

