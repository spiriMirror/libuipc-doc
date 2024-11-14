

# Class uipc::backend::DiffSimVisitor



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**backend**](namespaceuipc_1_1backend.md) **>** [**DiffSimVisitor**](classuipc_1_1backend_1_1_diff_sim_visitor.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DiffSimVisitor**](#function-diffsimvisitor) ([**core::DiffSim**](classuipc_1_1core_1_1_diff_sim.md) & diff\_sim) <br> |
|  void | [**H**](#function-h) (const [**diff\_sim::SparseCOOView**](classuipc_1_1diff__sim_1_1_sparse_c_o_o_view.md) & value) <br> |
|  void | [**need\_backend\_broadcast**](#function-need_backend_broadcast-12) (bool v) <br> |
|  bool | [**need\_backend\_broadcast**](#function-need_backend_broadcast-22) () const<br> |
|  void | [**need\_backend\_clear**](#function-need_backend_clear-12) (bool v) <br> |
|  bool | [**need\_backend\_clear**](#function-need_backend_clear-22) () const<br> |
|  void | [**pGpP**](#function-pgpp) (const [**diff\_sim::SparseCOOView**](classuipc_1_1diff__sim_1_1_sparse_c_o_o_view.md) & value) <br> |
|  [**diff\_sim::ParameterCollection**](classuipc_1_1diff__sim_1_1_parameter_collection.md) & | [**parameters**](#function-parameters-12) () <br> |
|  const [**diff\_sim::ParameterCollection**](classuipc_1_1diff__sim_1_1_parameter_collection.md) & | [**parameters**](#function-parameters-22) () const<br> |
|   | [**~DiffSimVisitor**](#function-diffsimvisitor) () <br> |




























## Public Functions Documentation




### function DiffSimVisitor 

```C++
uipc::backend::DiffSimVisitor::DiffSimVisitor (
    core::DiffSim & diff_sim
) 
```




<hr>



### function H 

```C++
void uipc::backend::DiffSimVisitor::H (
    const diff_sim::SparseCOOView & value
) 
```




<hr>



### function need\_backend\_broadcast [1/2]

```C++
void uipc::backend::DiffSimVisitor::need_backend_broadcast (
    bool v
) 
```




<hr>



### function need\_backend\_broadcast [2/2]

```C++
bool uipc::backend::DiffSimVisitor::need_backend_broadcast () const
```




<hr>



### function need\_backend\_clear [1/2]

```C++
void uipc::backend::DiffSimVisitor::need_backend_clear (
    bool v
) 
```




<hr>



### function need\_backend\_clear [2/2]

```C++
bool uipc::backend::DiffSimVisitor::need_backend_clear () const
```




<hr>



### function pGpP 

```C++
void uipc::backend::DiffSimVisitor::pGpP (
    const diff_sim::SparseCOOView & value
) 
```




<hr>



### function parameters [1/2]

```C++
diff_sim::ParameterCollection & uipc::backend::DiffSimVisitor::parameters () 
```




<hr>



### function parameters [2/2]

```C++
const diff_sim::ParameterCollection & uipc::backend::DiffSimVisitor::parameters () const
```




<hr>



### function ~DiffSimVisitor 

```C++
uipc::backend::DiffSimVisitor::~DiffSimVisitor () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/backend/visitors/diff_sim_visitor.h`

