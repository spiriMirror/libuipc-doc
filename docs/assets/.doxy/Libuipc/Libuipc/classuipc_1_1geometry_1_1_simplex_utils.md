

# Class uipc::geometry::SimplexUtils



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**SimplexUtils**](classuipc_1_1geometry_1_1_simplex_utils.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  bool | [**compare\_edge**](#function-compare_edge) (const Vector2i &, const Vector2i &) noexcept<br> |
|  bool | [**compare\_tet**](#function-compare_tet) (const Vector4i &, const Vector4i &) noexcept<br> |
|  bool | [**compare\_tri**](#function-compare_tri) (const Vector3i &, const Vector3i &) noexcept<br> |
|  bool | [**is\_same\_edge**](#function-is_same_edge) (const Vector2i &, const Vector2i &) noexcept<br> |
|  bool | [**is\_same\_oriented\_edge**](#function-is_same_oriented_edge) (const Vector2i &, const Vector2i &) noexcept<br> |
|  bool | [**is\_same\_oriented\_tet**](#function-is_same_oriented_tet) (const Vector4i &, const Vector4i &) noexcept<br> |
|  bool | [**is\_same\_oriented\_tri**](#function-is_same_oriented_tri) (const Vector3i &, const Vector3i &) noexcept<br> |
|  bool | [**is\_same\_tet**](#function-is_same_tet) (const Vector4i &, const Vector4i &) noexcept<br> |
|  bool | [**is\_same\_tri**](#function-is_same_tri) (const Vector3i &, const Vector3i &) noexcept<br> |
|  void | [**outward\_tri\_from\_tet**](#function-outward_tri_from_tet) (span&lt; const Vector3, 4 &gt; Vs, span&lt; Vector3i, 4 &gt; Fs) noexcept<br> |


























## Public Static Functions Documentation




### function compare\_edge 

```C++
static bool uipc::geometry::SimplexUtils::compare_edge (
    const Vector2i &,
    const Vector2i &
) noexcept
```




<hr>



### function compare\_tet 

```C++
static bool uipc::geometry::SimplexUtils::compare_tet (
    const Vector4i &,
    const Vector4i &
) noexcept
```




<hr>



### function compare\_tri 

```C++
static bool uipc::geometry::SimplexUtils::compare_tri (
    const Vector3i &,
    const Vector3i &
) noexcept
```




<hr>



### function is\_same\_edge 

```C++
static bool uipc::geometry::SimplexUtils::is_same_edge (
    const Vector2i &,
    const Vector2i &
) noexcept
```




<hr>



### function is\_same\_oriented\_edge 

```C++
static bool uipc::geometry::SimplexUtils::is_same_oriented_edge (
    const Vector2i &,
    const Vector2i &
) noexcept
```




<hr>



### function is\_same\_oriented\_tet 

```C++
static bool uipc::geometry::SimplexUtils::is_same_oriented_tet (
    const Vector4i &,
    const Vector4i &
) noexcept
```




<hr>



### function is\_same\_oriented\_tri 

```C++
static bool uipc::geometry::SimplexUtils::is_same_oriented_tri (
    const Vector3i &,
    const Vector3i &
) noexcept
```




<hr>



### function is\_same\_tet 

```C++
static bool uipc::geometry::SimplexUtils::is_same_tet (
    const Vector4i &,
    const Vector4i &
) noexcept
```




<hr>



### function is\_same\_tri 

```C++
static bool uipc::geometry::SimplexUtils::is_same_tri (
    const Vector3i &,
    const Vector3i &
) noexcept
```




<hr>



### function outward\_tri\_from\_tet 

```C++
static void uipc::geometry::SimplexUtils::outward_tri_from_tet (
    span< const Vector3, 4 > Vs,
    span< Vector3i, 4 > Fs
) noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/utils/simplex_utils.h`

