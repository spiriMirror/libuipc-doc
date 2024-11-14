

# Class uipc::diff\_sim::ParameterCollection



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**diff\_sim**](namespaceuipc_1_1diff__sim.md) **>** [**ParameterCollection**](classuipc_1_1diff__sim_1_1_parameter_collection.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**broadcast**](#function-broadcast) () <br>_Broadcast the parameter collection to corresponding geometry attributes._  |
|  void | [**resize**](#function-resize) (SizeT N, Float default\_value=0.0f) <br> |
|  span&lt; const Float &gt; | [**view**](#function-view-22) () const<br> |
|   | [**~ParameterCollection**](#function-parametercollection) () <br> |




























## Public Functions Documentation




### function broadcast 

```C++
void uipc::diff_sim::ParameterCollection::broadcast () 
```




<hr>



### function resize 

```C++
void uipc::diff_sim::ParameterCollection::resize (
    SizeT N,
    Float default_value=0.0f
) 
```




<hr>



### function view [2/2]

```C++
span< const Float > uipc::diff_sim::ParameterCollection::view () const
```




<hr>



### function ~ParameterCollection 

```C++
uipc::diff_sim::ParameterCollection::~ParameterCollection () 
```




<hr>## Friends Documentation





### friend DiffSimVisitor 

```C++
class uipc::diff_sim::ParameterCollection::DiffSimVisitor (
    uipc::backend::DiffSimVisitor
) 
```




<hr>



### friend DiffSim 

```C++
class uipc::diff_sim::ParameterCollection::DiffSim (
    uipc::core::DiffSim
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/diff_sim/parameter_collection.h`
