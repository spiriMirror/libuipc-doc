

# Class uipc::core::AffineBodyStateAccessorFeatureOverrider



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**AffineBodyStateAccessorFeatureOverrider**](classuipc_1_1core_1_1_affine_body_state_accessor_feature_overrider.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyStateAccessorFeatureOverrider**](#function-affinebodystateaccessorfeatureoverrider) () = default<br> |
| virtual void | [**do\_copy\_from**](#function-do_copy_from) (const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & state\_geo) = 0<br> |
| virtual void | [**do\_copy\_to**](#function-do_copy_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) & state\_geo) = 0<br> |
| virtual [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1_simplicial_complex.md) | [**do\_create\_geometry**](#function-do_create_geometry) (IndexT body\_offset, SizeT body\_count) <br> |
| virtual SizeT | [**get\_body\_count**](#function-get_body_count) () = 0<br> |
| virtual  | [**~AffineBodyStateAccessorFeatureOverrider**](#function-affinebodystateaccessorfeatureoverrider) () = default<br> |




























## Public Functions Documentation




### function AffineBodyStateAccessorFeatureOverrider 

```C++
uipc::core::AffineBodyStateAccessorFeatureOverrider::AffineBodyStateAccessorFeatureOverrider () = default
```




<hr>



### function do\_copy\_from 

```C++
virtual void uipc::core::AffineBodyStateAccessorFeatureOverrider::do_copy_from (
    const geometry::SimplicialComplex & state_geo
) = 0
```




<hr>



### function do\_copy\_to 

```C++
virtual void uipc::core::AffineBodyStateAccessorFeatureOverrider::do_copy_to (
    geometry::SimplicialComplex & state_geo
) = 0
```




<hr>



### function do\_create\_geometry 

```C++
virtual geometry::SimplicialComplex uipc::core::AffineBodyStateAccessorFeatureOverrider::do_create_geometry (
    IndexT body_offset,
    SizeT body_count
) 
```




<hr>



### function get\_body\_count 

```C++
virtual SizeT uipc::core::AffineBodyStateAccessorFeatureOverrider::get_body_count () = 0
```




<hr>



### function ~AffineBodyStateAccessorFeatureOverrider 

```C++
virtual uipc::core::AffineBodyStateAccessorFeatureOverrider::~AffineBodyStateAccessorFeatureOverrider () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/affine_body_state_accessor_feature.h`

