

# Class uipc::core::Animator



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**Animator**](classuipc_1_1core_1_1Animator.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Animator**](#function-animator-13) (const [**Animator**](classuipc_1_1core_1_1Animator.md) &) = delete<br> |
|   | [**Animator**](#function-animator-23) ([**Animator**](classuipc_1_1core_1_1Animator.md) &&) = delete<br> |
|  SizeT | [**animation\_count**](#function-animation_count) () noexcept const<br> |
|  vector&lt; IndexT &gt; | [**animation\_ids**](#function-animation_ids) () const<br> |
|  void | [**erase**](#function-erase) (IndexT id) <br> |
|  bool | [**has\_animation**](#function-has_animation) (IndexT id) noexcept const<br> |
|  void | [**insert**](#function-insert) ([**Object**](classuipc_1_1core_1_1Object.md) & obj, Animation::ActionOnUpdate && on\_update) <br> |
|  [**Animator**](classuipc_1_1core_1_1Animator.md) & | [**operator=**](#function-operator) (const [**Animator**](classuipc_1_1core_1_1Animator.md) &) = delete<br> |
|  [**Animator**](classuipc_1_1core_1_1Animator.md) & | [**operator=**](#function-operator_1) ([**Animator**](classuipc_1_1core_1_1Animator.md) &&) = delete<br> |
|  void | [**substep**](#function-substep-12) (SizeT n) <br> |
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



### function animation\_count 

```C++
SizeT uipc::core::Animator::animation_count () noexcept const
```




<hr>



### function animation\_ids 

```C++
vector< IndexT > uipc::core::Animator::animation_ids () const
```




<hr>



### function erase 

```C++
void uipc::core::Animator::erase (
    IndexT id
) 
```




<hr>



### function has\_animation 

```C++
bool uipc::core::Animator::has_animation (
    IndexT id
) noexcept const
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
) 
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



### friend Scene 

```C++
class uipc::core::Animator::Scene (
    internal::Scene
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/animator.h`

