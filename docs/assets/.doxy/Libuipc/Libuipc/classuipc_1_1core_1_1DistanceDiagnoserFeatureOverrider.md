

# Class uipc::core::DistanceDiagnoserFeatureOverrider



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**DistanceDiagnoserFeatureOverrider**](classuipc_1_1core_1_1DistanceDiagnoserFeatureOverrider.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_compute\_edge\_edge\_distance**](#function-do_compute_edge_edge_distance) ([**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & R, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & edges\_a, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & edges\_b, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & rest\_edges\_a, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & rest\_edges\_b) = 0<br> |
| virtual void | [**do\_compute\_point\_edge\_distance**](#function-do_compute_point_edge_distance) ([**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & R, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & points, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & edges) = 0<br> |
| virtual void | [**do\_compute\_point\_point\_distance**](#function-do_compute_point_point_distance) ([**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & R, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & points\_a, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & points\_b) = 0<br> |
| virtual void | [**do\_compute\_point\_triangle\_distance**](#function-do_compute_point_triangle_distance) ([**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & R, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & points, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & triangles) = 0<br> |
| virtual  | [**~DistanceDiagnoserFeatureOverrider**](#function-distancediagnoserfeatureoverrider) () = default<br> |




























## Public Functions Documentation




### function do\_compute\_edge\_edge\_distance 

```C++
virtual void uipc::core::DistanceDiagnoserFeatureOverrider::do_compute_edge_edge_distance (
    geometry::Geometry & R,
    const geometry::SimplicialComplex & edges_a,
    const geometry::SimplicialComplex & edges_b,
    const geometry::SimplicialComplex & rest_edges_a,
    const geometry::SimplicialComplex & rest_edges_b
) = 0
```




<hr>



### function do\_compute\_point\_edge\_distance 

```C++
virtual void uipc::core::DistanceDiagnoserFeatureOverrider::do_compute_point_edge_distance (
    geometry::Geometry & R,
    const geometry::SimplicialComplex & points,
    const geometry::SimplicialComplex & edges
) = 0
```




<hr>



### function do\_compute\_point\_point\_distance 

```C++
virtual void uipc::core::DistanceDiagnoserFeatureOverrider::do_compute_point_point_distance (
    geometry::Geometry & R,
    const geometry::SimplicialComplex & points_a,
    const geometry::SimplicialComplex & points_b
) = 0
```




<hr>



### function do\_compute\_point\_triangle\_distance 

```C++
virtual void uipc::core::DistanceDiagnoserFeatureOverrider::do_compute_point_triangle_distance (
    geometry::Geometry & R,
    const geometry::SimplicialComplex & points,
    const geometry::SimplicialComplex & triangles
) = 0
```




<hr>



### function ~DistanceDiagnoserFeatureOverrider 

```C++
virtual uipc::core::DistanceDiagnoserFeatureOverrider::~DistanceDiagnoserFeatureOverrider () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/distance_diagnoser_feature.h`

