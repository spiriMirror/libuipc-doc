

# Struct uipc::PmrDeleter

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**PmrDeleter**](structuipc_1_1PmrDeleter.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef uipc::Allocator&lt; T &gt; | [**Allocator**](#typedef-allocator)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**operator()**](#function-operator) (T \* ptr) const<br> |




























## Public Types Documentation




### typedef Allocator 

```C++
using uipc::PmrDeleter< T >::Allocator =  uipc::Allocator<T>;
```




<hr>
## Public Functions Documentation




### function operator() 

```C++
void uipc::PmrDeleter::operator() (
    T * ptr
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/smart_pointer.h`

