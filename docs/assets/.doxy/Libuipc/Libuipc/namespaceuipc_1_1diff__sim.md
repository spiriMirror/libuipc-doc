

# Namespace uipc::diff\_sim



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**diff\_sim**](namespaceuipc_1_1diff__sim.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**AdjointMethodFeature**](classuipc_1_1diff__sim_1_1AdjointMethodFeature.md) <br> |
| class | [**AdjointMethodFeatureOverrider**](classuipc_1_1diff__sim_1_1AdjointMethodFeatureOverrider.md) <br> |
| class | [**EnableGradFeature**](classuipc_1_1diff__sim_1_1EnableGradFeature.md) <br> |
| class | [**EnableGradFeatureOverrider**](classuipc_1_1diff__sim_1_1EnableGradFeatureOverrider.md) <br> |
| class | [**ParameterCollection**](classuipc_1_1diff__sim_1_1ParameterCollection.md) <br> |
| class | [**SparseCOOView**](classuipc_1_1diff__sim_1_1SparseCOOView.md) <br> |






















## Public Functions

| Type | Name |
| ---: | :--- |
|  UIPC\_CORE\_API Eigen::Map&lt; Eigen::Matrix&lt; Float, Eigen::Dynamic, 1 &gt; &gt; | [**as\_eigen**](#function-as_eigen) ([**ParameterCollection**](classuipc_1_1diff__sim_1_1ParameterCollection.md) & collection) <br> |
|  UIPC\_CORE\_API span&lt; Float &gt; | [**view**](#function-view) ([**ParameterCollection**](classuipc_1_1diff__sim_1_1ParameterCollection.md) & collection) <br> |




























## Public Functions Documentation




### function as\_eigen 

```C++
UIPC_CORE_API Eigen::Map< Eigen::Matrix< Float, Eigen::Dynamic, 1 > > uipc::diff_sim::as_eigen (
    ParameterCollection & collection
) 
```




<hr>



### function view 

```C++
UIPC_CORE_API span< Float > uipc::diff_sim::view (
    ParameterCollection & collection
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/diff_sim/adjoint_method_feature.h`

