

# Class uipc::diff\_sim::EnableGradFeature



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**diff\_sim**](namespaceuipc_1_1diff__sim.md) **>** [**EnableGradFeature**](classuipc_1_1diff__sim_1_1_enable_grad_feature.md)








Inherits the following classes: [uipc::core::Feature](classuipc_1_1core_1_1_feature.md)
































## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**FeatureName**](#variable-featurename)   = `"diff\_sim/enable\_grad"`<br> |










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**EnableGradFeature**](#function-enablegradfeature) (S&lt; [**EnableGradFeatureOverrider**](classuipc_1_1diff__sim_1_1_enable_grad_feature_overrider.md) &gt; overrider) <br> |
|  bool | [**is\_grad\_enabled**](#function-is_grad_enabled) () const<br>_Check if parameter gradient computation is enabled._  |
|  void | [**no\_grad**](#function-no_grad) () <br>_With DiffSim on, turn off parameter gradient computation._  |
|  void | [**with\_grad**](#function-with_grad) () <br>_With DiffSim on, turn on parameter gradient computation._  |




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
| virtual std::string\_view | [**get\_name**](classuipc_1_1core_1_1_i_feature.md#function-get_name) () const = 0<br> |
| virtual std::string\_view | [**get\_type\_name**](classuipc_1_1core_1_1_i_feature.md#function-get_type_name) () const = 0<br> |








## Public Static Attributes Documentation




### variable FeatureName 

```C++
std::string_view uipc::diff_sim::EnableGradFeature::FeatureName;
```




<hr>
## Public Functions Documentation




### function EnableGradFeature 

```C++
uipc::diff_sim::EnableGradFeature::EnableGradFeature (
    S< EnableGradFeatureOverrider > overrider
) 
```




<hr>



### function is\_grad\_enabled 

_Check if parameter gradient computation is enabled._ 
```C++
bool uipc::diff_sim::EnableGradFeature::is_grad_enabled () const
```





**Returns:**

true if parameter gradient computation is enabled. 





        

<hr>



### function no\_grad 

_With DiffSim on, turn off parameter gradient computation._ 
```C++
void uipc::diff_sim::EnableGradFeature::no_grad () 
```




<hr>



### function with\_grad 

_With DiffSim on, turn on parameter gradient computation._ 
```C++
void uipc::diff_sim::EnableGradFeature::with_grad () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/diff_sim/enable_grad_feature.h`

