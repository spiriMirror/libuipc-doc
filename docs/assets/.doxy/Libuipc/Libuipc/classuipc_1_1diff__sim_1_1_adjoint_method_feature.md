

# Class uipc::diff\_sim::AdjointMethodFeature



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**diff\_sim**](namespaceuipc_1_1diff__sim.md) **>** [**AdjointMethodFeature**](classuipc_1_1diff__sim_1_1_adjoint_method_feature.md)








Inherits the following classes: [uipc::core::Feature](classuipc_1_1core_1_1_feature.md)
































## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**FeatureName**](#variable-featurename)   = `"diff\_sim/adjoint\_method"`<br> |










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AdjointMethodFeature**](#function-adjointmethodfeature) (S&lt; [**AdjointMethodFeatureOverrider**](classuipc_1_1diff__sim_1_1_adjoint_method_feature_overrider.md) &gt; overrider) <br> |
|  void | [**compute\_dLdP**](#function-compute_dldp) ([**backend::BufferView**](classuipc_1_1backend_1_1_buffer_view.md) out\_dLdP, [**backend::BufferView**](classuipc_1_1backend_1_1_buffer_view.md) in\_dLdX) <br>_Computes the gradient of the loss with respect to the parameters._  |
|  void | [**receive\_dofs**](#function-receive_dofs) ([**backend::BufferView**](classuipc_1_1backend_1_1_buffer_view.md) out\_Dofs) <br>_Receives the selected degrees of freedom for all frames._  |
|  void | [**select\_dofs**](#function-select_dofs) (SizeT frame, [**backend::BufferView**](classuipc_1_1backend_1_1_buffer_view.md) in\_SDI) <br>_Selects the degrees of freedom from the given indices for the given frame._  |




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








## Public Static Attributes Documentation




### variable FeatureName 

```C++
std::string_view uipc::diff_sim::AdjointMethodFeature::FeatureName;
```




<hr>
## Public Functions Documentation




### function AdjointMethodFeature 

```C++
uipc::diff_sim::AdjointMethodFeature::AdjointMethodFeature (
    S< AdjointMethodFeatureOverrider > overrider
) 
```




<hr>



### function compute\_dLdP 

_Computes the gradient of the loss with respect to the parameters._ 
```C++
void uipc::diff_sim::AdjointMethodFeature::compute_dLdP (
    backend::BufferView out_dLdP,
    backend::BufferView in_dLdX
) 
```





**Parameters:**


* `out_dLdP:BufferView<Float>` The gradient of the loss with respect to the parameters. 
* `in_dLdX:BufferView<Float>` The gradient of the loss with respect to the degrees of freedom. 




        

<hr>



### function receive\_dofs 

_Receives the selected degrees of freedom for all frames._ 
```C++
void uipc::diff_sim::AdjointMethodFeature::receive_dofs (
    backend::BufferView out_Dofs
) 
```



This function should be called after all frames have been processed to receive the selected degrees of freedom.




**Parameters:**


* `out_dofs:BufferView<Float>` The selected degrees of freedom. 




        

<hr>



### function select\_dofs 

_Selects the degrees of freedom from the given indices for the given frame._ 
```C++
void uipc::diff_sim::AdjointMethodFeature::select_dofs (
    SizeT frame,
    backend::BufferView in_SDI
) 
```



`in_SDI` is frame-local, this function should be called for each frame to select the degrees of freedom.




**Parameters:**


* `in_SDI:BufferView<IndexT>` The indices of the degrees of freedom to select. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/diff_sim/adjoint_method_feature.h`

