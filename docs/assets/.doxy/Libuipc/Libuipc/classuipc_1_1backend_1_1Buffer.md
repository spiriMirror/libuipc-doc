

# Class uipc::backend::Buffer



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**backend**](namespaceuipc_1_1backend.md) **>** [**Buffer**](classuipc_1_1backend_1_1Buffer.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Buffer**](#function-buffer) (std::function&lt; void(SizeT)&gt; resize\_func, std::function&lt; [**BufferView**](classuipc_1_1backend_1_1BufferView.md)()&gt; get\_buffer\_view\_func) <br> |
|  void | [**resize**](#function-resize) (SizeT size) <br> |
|  [**BufferView**](classuipc_1_1backend_1_1BufferView.md) | [**view**](#function-view) () const<br> |




























## Public Functions Documentation




### function Buffer 

```C++
uipc::backend::Buffer::Buffer (
    std::function< void(SizeT)> resize_func,
    std::function< BufferView ()> get_buffer_view_func
) 
```




<hr>



### function resize 

```C++
void uipc::backend::Buffer::resize (
    SizeT size
) 
```




<hr>



### function view 

```C++
BufferView uipc::backend::Buffer::view () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/backend/buffer.h`

