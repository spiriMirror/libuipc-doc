

# Class uipc::core::Animation



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**Animation**](classuipc_1_1core_1_1_animation.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**UpdateHint**](classuipc_1_1core_1_1_animation_1_1_update_hint.md) <br> |
| class | [**UpdateInfo**](classuipc_1_1core_1_1_animation_1_1_update_info.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::function&lt; void([**UpdateInfo**](classuipc_1_1core_1_1_animation_1_1_update_info.md) &)&gt; | [**ActionOnUpdate**](#typedef-actiononupdate)  <br> |
















































## Public Types Documentation




### typedef ActionOnUpdate 

```C++
using uipc::core::Animation::ActionOnUpdate =  std::function<void(UpdateInfo&)>;
```




<hr>## Friends Documentation





### friend AnimatorVisitor 

```C++
class uipc::core::Animation::AnimatorVisitor (
    backend::AnimatorVisitor
) 
```




<hr>



### friend formatter&lt; Animation &gt; 

```C++
struct uipc::core::Animation::formatter< Animation > (
    fmt::formatter< Animation >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/animation.h`

