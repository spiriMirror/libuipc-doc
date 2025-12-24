

# Class uipc::core::ContactSystemFeature



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ContactSystemFeature**](classuipc_1_1core_1_1ContactSystemFeature.md)








Inherits the following classes: [uipc::core::Feature](classuipc_1_1core_1_1Feature.md)
































## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  constexpr std::string\_view | [**FeatureName**](#variable-featurename)   = `"core/contact\_system"`<br> |










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ContactSystemFeature**](#function-contactsystemfeature) (S&lt; [**ContactSystemFeatureOverrider**](classuipc_1_1core_1_1ContactSystemFeatureOverrider.md) &gt; overrider) <br> |
|  void | [**contact\_energy**](#function-contact_energy-12) (std::string\_view prim\_type, [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & energy) <br> |
|  void | [**contact\_energy**](#function-contact_energy-22) (const [**constitution::IConstitution**](classuipc_1_1constitution_1_1IConstitution.md) & c, [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & energy) <br> |
|  void | [**contact\_gradient**](#function-contact_gradient-12) (std::string\_view prim\_type, [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & vert\_grad) <br> |
|  void | [**contact\_gradient**](#function-contact_gradient-22) (const [**constitution::IConstitution**](classuipc_1_1constitution_1_1IConstitution.md) & c, [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & vert\_grad) <br> |
|  void | [**contact\_hessian**](#function-contact_hessian-12) (std::string\_view prim\_type, [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & vert\_hess) <br> |
|  void | [**contact\_hessian**](#function-contact_hessian-22) (const [**constitution::IConstitution**](classuipc_1_1constitution_1_1IConstitution.md) & c, [**geometry::Geometry**](classuipc_1_1geometry_1_1Geometry.md) & vert\_hess) <br> |
|  vector&lt; std::string &gt; | [**contact\_primitive\_types**](#function-contact_primitive_types) () const<br> |




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
constexpr std::string_view uipc::core::ContactSystemFeature::FeatureName;
```




<hr>
## Public Functions Documentation




### function ContactSystemFeature 

```C++
uipc::core::ContactSystemFeature::ContactSystemFeature (
    S< ContactSystemFeatureOverrider > overrider
) 
```




<hr>



### function contact\_energy [1/2]

```C++
void uipc::core::ContactSystemFeature::contact_energy (
    std::string_view prim_type,
    geometry::Geometry & energy
) 
```




<hr>



### function contact\_energy [2/2]

```C++
void uipc::core::ContactSystemFeature::contact_energy (
    const constitution::IConstitution & c,
    geometry::Geometry & energy
) 
```




<hr>



### function contact\_gradient [1/2]

```C++
void uipc::core::ContactSystemFeature::contact_gradient (
    std::string_view prim_type,
    geometry::Geometry & vert_grad
) 
```




<hr>



### function contact\_gradient [2/2]

```C++
void uipc::core::ContactSystemFeature::contact_gradient (
    const constitution::IConstitution & c,
    geometry::Geometry & vert_grad
) 
```




<hr>



### function contact\_hessian [1/2]

```C++
void uipc::core::ContactSystemFeature::contact_hessian (
    std::string_view prim_type,
    geometry::Geometry & vert_hess
) 
```




<hr>



### function contact\_hessian [2/2]

```C++
void uipc::core::ContactSystemFeature::contact_hessian (
    const constitution::IConstitution & c,
    geometry::Geometry & vert_hess
) 
```




<hr>



### function contact\_primitive\_types 

```C++
vector< std::string > uipc::core::ContactSystemFeature::contact_primitive_types () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/contact_system_feature.h`

