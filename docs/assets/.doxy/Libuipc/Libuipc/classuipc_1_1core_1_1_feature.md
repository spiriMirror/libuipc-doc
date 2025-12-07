

# Class uipc::core::Feature



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**Feature**](classuipc_1_1core_1_1_feature.md)








Inherits the following classes: [uipc::core::IFeature](classuipc_1_1core_1_1_i_feature.md)


Inherited by the following classes: [uipc::core::AffineBodyStateAccessorFeature](classuipc_1_1core_1_1_affine_body_state_accessor_feature.md),  [uipc::core::ContactSystemFeature](classuipc_1_1core_1_1_contact_system_feature.md),  [uipc::core::FiniteElementStateAccessorFeature](classuipc_1_1core_1_1_finite_element_state_accessor_feature.md),  [uipc::diff\_sim::AdjointMethodFeature](classuipc_1_1diff__sim_1_1_adjoint_method_feature.md),  [uipc::diff\_sim::EnableGradFeature](classuipc_1_1diff__sim_1_1_enable_grad_feature.md)






















































## Public Functions inherited from uipc::core::IFeature

See [uipc::core::IFeature](classuipc_1_1core_1_1_i_feature.md)

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**name**](classuipc_1_1core_1_1_i_feature.md#function-name) () const<br> |
|  std::string\_view | [**type\_name**](classuipc_1_1core_1_1_i_feature.md#function-type_name) () const<br> |
| virtual  | [**~IFeature**](classuipc_1_1core_1_1_i_feature.md#function-ifeature) () = default<br> |
















































## Protected Functions inherited from uipc::core::IFeature

See [uipc::core::IFeature](classuipc_1_1core_1_1_i_feature.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_on\_required**](classuipc_1_1core_1_1_i_feature.md#function-do_on_required) () const = 0<br> |
| virtual std::string\_view | [**get\_name**](classuipc_1_1core_1_1_i_feature.md#function-get_name) () const = 0<br> |
| virtual std::string\_view | [**get\_type\_name**](classuipc_1_1core_1_1_i_feature.md#function-get_type_name) () const = 0<br> |







------------------------------
The documentation for this class was generated from the following file `include/uipc/core/feature.h`

