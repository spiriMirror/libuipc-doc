

# Namespace uipc::geometry::detail



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**detail**](namespaceuipc_1_1geometry_1_1detail.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  span&lt; Vector3 &gt; | [**resize\_positions**](#function-resize_positions) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, SizeT count) <br> |
|  auto | [**resize\_topology**](#function-resize_topology) ([**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1SimplicialComplexAttributes.md)&lt; false, N &gt; facets, SizeT count) <br> |
|  void | [**triangulate\_quads**](#function-triangulate_quads) ([**SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, const Quads & quads) <br> |




























## Public Functions Documentation




### function resize\_positions 

```C++
inline span< Vector3 > uipc::geometry::detail::resize_positions (
    SimplicialComplex & sc,
    SizeT count
) 
```




<hr>



### function resize\_topology 

```C++
template<IndexT N>
auto uipc::geometry::detail::resize_topology (
    SimplicialComplexAttributes < false, N > facets,
    SizeT count
) 
```




<hr>



### function triangulate\_quads 

```C++
template<typename Quads>
void uipc::geometry::detail::triangulate_quads (
    SimplicialComplex & sc,
    const Quads & quads
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/details/factory.h`

