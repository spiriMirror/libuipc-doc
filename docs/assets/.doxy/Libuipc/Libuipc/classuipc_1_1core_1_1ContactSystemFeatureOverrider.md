

# Class uipc::core::ContactSystemFeatureOverrider



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ContactSystemFeatureOverrider**](classuipc_1_1core_1_1ContactSystemFeatureOverrider.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**get\_contact\_energy**](#function-get_contact_energy) (std::string\_view prim\_type, [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & energy\_geo) = 0<br> |
| virtual void | [**get\_contact\_gradient**](#function-get_contact_gradient) (std::string\_view prim\_type, [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & vert\_grad) = 0<br> |
| virtual void | [**get\_contact\_hessian**](#function-get_contact_hessian) (std::string\_view prim\_type, [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & vert\_hess) = 0<br> |
| virtual vector&lt; std::string &gt; | [**get\_contact\_primitive\_types**](#function-get_contact_primitive_types) () const = 0<br> |




























## Public Functions Documentation




### function get\_contact\_energy 

```C++
virtual void uipc::core::ContactSystemFeatureOverrider::get_contact_energy (
    std::string_view prim_type,
    geometry::Geometry & energy_geo
) = 0
```




<hr>



### function get\_contact\_gradient 

```C++
virtual void uipc::core::ContactSystemFeatureOverrider::get_contact_gradient (
    std::string_view prim_type,
    geometry::Geometry & vert_grad
) = 0
```




<hr>



### function get\_contact\_hessian 

```C++
virtual void uipc::core::ContactSystemFeatureOverrider::get_contact_hessian (
    std::string_view prim_type,
    geometry::Geometry & vert_hess
) = 0
```




<hr>



### function get\_contact\_primitive\_types 

```C++
virtual vector< std::string > uipc::core::ContactSystemFeatureOverrider::get_contact_primitive_types () const = 0
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/contact_system_feature.h`

