

# Class uipc::core::DistanceDiagnoserFeature



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**DistanceDiagnoserFeature**](classuipc_1_1core_1_1DistanceDiagnoserFeature.md)








Inherits the following classes: [uipc::core::Feature](classuipc_1_1core_1_1Feature.md)
































## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  constexpr std::string\_view | [**FeatureName**](#variable-featurename)   = `"core/distance\_diagnoser"`<br> |










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DistanceDiagnoserFeature**](#function-distancediagnoserfeature) (S&lt; [**DistanceDiagnoserFeatureOverrider**](classuipc_1_1core_1_1DistanceDiagnoserFeatureOverrider.md) &gt; overrider) <br> |
|  void | [**compute\_edge\_edge\_distance**](#function-compute_edge_edge_distance) ([**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & R, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & edges\_a, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & edges\_b, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & rest\_edges\_a, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & rest\_edges\_b) <br> |
|  void | [**compute\_point\_edge\_distance**](#function-compute_point_edge_distance) ([**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & R, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & points, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & edges) <br> |
|  void | [**compute\_point\_point\_distance**](#function-compute_point_point_distance) ([**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & R, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & points\_a, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & points\_b) <br> |
|  void | [**compute\_point\_triangle\_distance**](#function-compute_point_triangle_distance) ([**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & R, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & points, const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & triangles) <br> |




## Public Functions inherited from uipc::core::IFeature

See [uipc::core::IFeature](classuipc_1_1core_1_1IFeature.md)

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**name**](classuipc_1_1core_1_1IFeature.md#function-name) () const<br> |
|  std::string\_view | [**type\_name**](classuipc_1_1core_1_1IFeature.md#function-type_name) () const<br> |
| virtual  | [**~IFeature**](classuipc_1_1core_1_1IFeature.md#function-ifeature) () = default<br> |








































































## Protected Functions inherited from uipc::core::IFeature

See [uipc::core::IFeature](classuipc_1_1core_1_1IFeature.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_on\_required**](classuipc_1_1core_1_1IFeature.md#function-do_on_required) () const = 0<br> |
| virtual std::string\_view | [**get\_name**](classuipc_1_1core_1_1IFeature.md#function-get_name) () const = 0<br> |
| virtual std::string\_view | [**get\_type\_name**](classuipc_1_1core_1_1IFeature.md#function-get_type_name) () const = 0<br> |








## Public Static Attributes Documentation




### variable FeatureName 

```C++
constexpr std::string_view uipc::core::DistanceDiagnoserFeature::FeatureName;
```




<hr>
## Public Functions Documentation




### function DistanceDiagnoserFeature 

```C++
uipc::core::DistanceDiagnoserFeature::DistanceDiagnoserFeature (
    S< DistanceDiagnoserFeatureOverrider > overrider
) 
```




<hr>



### function compute\_edge\_edge\_distance 

```C++
void uipc::core::DistanceDiagnoserFeature::compute_edge_edge_distance (
    geometry::Geometry & R,
    const geometry::SimplicialComplex & edges_a,
    const geometry::SimplicialComplex & edges_b,
    const geometry::SimplicialComplex & rest_edges_a,
    const geometry::SimplicialComplex & rest_edges_b
) 
```




<hr>



### function compute\_point\_edge\_distance 

```C++
void uipc::core::DistanceDiagnoserFeature::compute_point_edge_distance (
    geometry::Geometry & R,
    const geometry::SimplicialComplex & points,
    const geometry::SimplicialComplex & edges
) 
```




<hr>



### function compute\_point\_point\_distance 

```C++
void uipc::core::DistanceDiagnoserFeature::compute_point_point_distance (
    geometry::Geometry & R,
    const geometry::SimplicialComplex & points_a,
    const geometry::SimplicialComplex & points_b
) 
```




<hr>



### function compute\_point\_triangle\_distance 

```C++
void uipc::core::DistanceDiagnoserFeature::compute_point_triangle_distance (
    geometry::Geometry & R,
    const geometry::SimplicialComplex & points,
    const geometry::SimplicialComplex & triangles
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/distance_diagnoser_feature.h`

