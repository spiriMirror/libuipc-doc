

# Class uipc::core::FiniteElementStateAccessorFeatureOverrider



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**FiniteElementStateAccessorFeatureOverrider**](classuipc_1_1core_1_1_finite_element_state_accessor_feature_overrider.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_copy\_from**](#function-do_copy_from) (const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & state\_geo) = 0<br> |
| virtual void | [**do\_copy\_to**](#function-do_copy_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & state\_geo) = 0<br> |
| virtual [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**do\_create\_geometry**](#function-do_create_geometry) (IndexT vertex\_offset, SizeT vertex\_count) <br> |
| virtual SizeT | [**get\_vertex\_count**](#function-get_vertex_count) () = 0<br> |
| virtual  | [**~FiniteElementStateAccessorFeatureOverrider**](#function-finiteelementstateaccessorfeatureoverrider) () = default<br> |




























## Public Functions Documentation




### function do\_copy\_from 

```C++
virtual void uipc::core::FiniteElementStateAccessorFeatureOverrider::do_copy_from (
    const geometry::SimplicialComplex & state_geo
) = 0
```




<hr>



### function do\_copy\_to 

```C++
virtual void uipc::core::FiniteElementStateAccessorFeatureOverrider::do_copy_to (
    geometry::SimplicialComplex & state_geo
) = 0
```




<hr>



### function do\_create\_geometry 

```C++
virtual geometry::SimplicialComplex uipc::core::FiniteElementStateAccessorFeatureOverrider::do_create_geometry (
    IndexT vertex_offset,
    SizeT vertex_count
) 
```




<hr>



### function get\_vertex\_count 

```C++
virtual SizeT uipc::core::FiniteElementStateAccessorFeatureOverrider::get_vertex_count () = 0
```




<hr>



### function ~FiniteElementStateAccessorFeatureOverrider 

```C++
virtual uipc::core::FiniteElementStateAccessorFeatureOverrider::~FiniteElementStateAccessorFeatureOverrider () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/finite_element_state_accessor_feature.h`

