

# Class uipc::diff\_sim::AdjointMethodFeatureOverrider



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**diff\_sim**](namespaceuipc_1_1diff__sim.md) **>** [**AdjointMethodFeatureOverrider**](classuipc_1_1diff__sim_1_1_adjoint_method_feature_overrider.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_compute\_dLdP**](#function-do_compute_dldp) ([**backend::BufferView**](classuipc_1_1backend_1_1_buffer_view.md) out\_dLdP, [**backend::BufferView**](classuipc_1_1backend_1_1_buffer_view.md) in\_dLdx) = 0<br> |
| virtual void | [**do\_receive\_dofs**](#function-do_receive_dofs) ([**backend::BufferView**](classuipc_1_1backend_1_1_buffer_view.md) out\_dofs) = 0<br> |
| virtual void | [**do\_select\_dofs**](#function-do_select_dofs) (SizeT frame, [**backend::BufferView**](classuipc_1_1backend_1_1_buffer_view.md) in\_SDI) = 0<br> |




























## Public Functions Documentation




### function do\_compute\_dLdP 

```C++
virtual void uipc::diff_sim::AdjointMethodFeatureOverrider::do_compute_dLdP (
    backend::BufferView out_dLdP,
    backend::BufferView in_dLdx
) = 0
```




<hr>



### function do\_receive\_dofs 

```C++
virtual void uipc::diff_sim::AdjointMethodFeatureOverrider::do_receive_dofs (
    backend::BufferView out_dofs
) = 0
```




<hr>



### function do\_select\_dofs 

```C++
virtual void uipc::diff_sim::AdjointMethodFeatureOverrider::do_select_dofs (
    SizeT frame,
    backend::BufferView in_SDI
) = 0
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/diff_sim/adjoint_method_feature.h`

