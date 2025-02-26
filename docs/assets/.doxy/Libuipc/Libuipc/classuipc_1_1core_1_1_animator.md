

# Class uipc::core::Animator



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**Animator**](classuipc_1_1core_1_1_animator.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Animator**](#function-animator-13) (const [**Animator**](classuipc_1_1core_1_1_animator.md) &) = delete<br> |
|   | [**Animator**](#function-animator-23) ([**Animator**](classuipc_1_1core_1_1_animator.md) &&) = delete<br> |
|  void | [**erase**](#function-erase) (IndexT id) <br> |
|  void | [**insert**](#function-insert) ([**Object**](classuipc_1_1core_1_1_object.md) & obj, Animation::ActionOnUpdate && on\_update) <br> |
|  [**Animator**](classuipc_1_1core_1_1_animator.md) & | [**operator=**](#function-operator) (const [**Animator**](classuipc_1_1core_1_1_animator.md) &) = delete<br> |
|  [**Animator**](classuipc_1_1core_1_1_animator.md) & | [**operator=**](#function-operator_1) ([**Animator**](classuipc_1_1core_1_1_animator.md) &&) = delete<br> |
|  void | [**substep**](#function-substep-12) (SizeT n) noexcept<br> |
|  SizeT | [**substep**](#function-substep-22) () noexcept const<br> |




























## Public Functions Documentation




### function Animator [1/3]

```C++
uipc::core::Animator::Animator (
    const Animator &
) = delete
```




<hr>



### function Animator [2/3]

```C++
uipc::core::Animator::Animator (
    Animator &&
) = delete
```




<hr>



### function erase 

```C++
void uipc::core::Animator::erase (
    IndexT id
) 
```




<hr>



### function insert 

```C++
void uipc::core::Animator::insert (
    Object & obj,
    Animation::ActionOnUpdate && on_update
) 
```




<hr>



### function operator= 

```C++
Animator & uipc::core::Animator::operator= (
    const Animator &
) = delete
```




<hr>



### function operator= 

```C++
Animator & uipc::core::Animator::operator= (
    Animator &&
) = delete
```




<hr>



### function substep [1/2]

```C++
void uipc::core::Animator::substep (
    SizeT n
) noexcept
```




<hr>



### function substep [2/2]

```C++
SizeT uipc::core::Animator::substep () noexcept const
```




<hr>## Friends Documentation





### friend AnimatorVisitor 

```C++
class uipc::core::Animator::AnimatorVisitor (
    backend::AnimatorVisitor
) 
```




<hr>



### friend formatter&lt; Animator &gt; 

```C++
struct uipc::core::Animator::formatter< Animator > (
    fmt::formatter< Animator >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/animator.h`

