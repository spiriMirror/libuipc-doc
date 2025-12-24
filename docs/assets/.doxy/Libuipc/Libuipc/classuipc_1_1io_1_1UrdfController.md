

# Class uipc::io::UrdfController



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**io**](namespaceuipc_1_1io.md) **>** [**UrdfController**](classuipc_1_1io_1_1UrdfController.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**UrdfController**](#function-urdfcontroller-13) (const [**UrdfController**](classuipc_1_1io_1_1UrdfController.md) & other) <br> |
|   | [**UrdfController**](#function-urdfcontroller-23) ([**UrdfController**](classuipc_1_1io_1_1UrdfController.md) && other) = default<br> |
|  void | [**apply\_to**](#function-apply_to) (std::string\_view attr) const<br> |
|  vector&lt; S&lt; [**geometry::SimplicialComplexSlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01SimplicialComplex_01_4.md) &gt; &gt; | [**links**](#function-links) () const<br> |
|  void | [**move\_root**](#function-move_root) (const Vector3 & xyz, const Vector3 & rpy) const<br> |
|  S&lt; [**geometry::ImplicitGeometrySlot**](classuipc_1_1geometry_1_1GeometrySlotT_3_01ImplicitGeometry_01_4.md) &gt; | [**revolute\_joints**](#function-revolute_joints) () const<br> |
|  void | [**rotate\_to**](#function-rotate_to) (std::string\_view joint\_name, Float angle) const<br> |
|  void | [**sync\_visual\_mesh**](#function-sync_visual_mesh) () const<br> |
|   | [**~UrdfController**](#function-urdfcontroller) () <br> |




























## Public Functions Documentation




### function UrdfController [1/3]

```C++
uipc::io::UrdfController::UrdfController (
    const UrdfController & other
) 
```




<hr>



### function UrdfController [2/3]

```C++
uipc::io::UrdfController::UrdfController (
    UrdfController && other
) = default
```




<hr>



### function apply\_to 

```C++
void uipc::io::UrdfController::apply_to (
    std::string_view attr
) const
```




<hr>



### function links 

```C++
vector< S< geometry::SimplicialComplexSlot > > uipc::io::UrdfController::links () const
```




<hr>



### function move\_root 

```C++
void uipc::io::UrdfController::move_root (
    const Vector3 & xyz,
    const Vector3 & rpy
) const
```




<hr>



### function revolute\_joints 

```C++
S< geometry::ImplicitGeometrySlot > uipc::io::UrdfController::revolute_joints () const
```




<hr>



### function rotate\_to 

```C++
void uipc::io::UrdfController::rotate_to (
    std::string_view joint_name,
    Float angle
) const
```




<hr>



### function sync\_visual\_mesh 

```C++
void uipc::io::UrdfController::sync_visual_mesh () const
```




<hr>



### function ~UrdfController 

```C++
uipc::io::UrdfController::~UrdfController () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/io/urdf_io.h`

