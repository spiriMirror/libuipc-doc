

# Class uipc::backend::BufferView



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**backend**](namespaceuipc_1_1backend.md) **>** [**BufferView**](classuipc_1_1backend_1_1_buffer_view.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**BufferView**](#function-bufferview-12) () = default<br> |
|   | [**BufferView**](#function-bufferview-22) (HandleT handle, SizeT element\_offset, SizeT element\_count, SizeT element\_size, SizeT element\_stride, std::string\_view backend\_name) noexcept<br> |
|  std::string\_view | [**backend**](#function-backend) () noexcept const<br> |
|  SizeT | [**element\_size**](#function-element_size) () noexcept const<br> |
|  SizeT | [**element\_stride**](#function-element_stride) () noexcept const<br> |
|  HandleT | [**handle**](#function-handle) () noexcept const<br> |
|  SizeT | [**offset**](#function-offset) () noexcept const<br> |
|   | [**operator bool**](#function-operator-bool) () noexcept const<br> |
|  SizeT | [**size**](#function-size) () noexcept const<br> |
|  SizeT | [**size\_in\_bytes**](#function-size_in_bytes) () noexcept const<br> |
|  [**BufferView**](classuipc_1_1backend_1_1_buffer_view.md) | [**subview**](#function-subview) (SizeT offset, SizeT element\_count) noexcept const<br> |




























## Public Functions Documentation




### function BufferView [1/2]

```C++
uipc::backend::BufferView::BufferView () = default
```




<hr>



### function BufferView [2/2]

```C++
uipc::backend::BufferView::BufferView (
    HandleT handle,
    SizeT element_offset,
    SizeT element_count,
    SizeT element_size,
    SizeT element_stride,
    std::string_view backend_name
) noexcept
```




<hr>



### function backend 

```C++
std::string_view uipc::backend::BufferView::backend () noexcept const
```




<hr>



### function element\_size 

```C++
SizeT uipc::backend::BufferView::element_size () noexcept const
```




<hr>



### function element\_stride 

```C++
SizeT uipc::backend::BufferView::element_stride () noexcept const
```




<hr>



### function handle 

```C++
HandleT uipc::backend::BufferView::handle () noexcept const
```




<hr>



### function offset 

```C++
SizeT uipc::backend::BufferView::offset () noexcept const
```




<hr>



### function operator bool 

```C++
uipc::backend::BufferView::operator bool () noexcept const
```




<hr>



### function size 

```C++
SizeT uipc::backend::BufferView::size () noexcept const
```




<hr>



### function size\_in\_bytes 

```C++
SizeT uipc::backend::BufferView::size_in_bytes () noexcept const
```




<hr>



### function subview 

```C++
BufferView uipc::backend::BufferView::subview (
    SizeT offset,
    SizeT element_count
) noexcept const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/backend/buffer_view.h`

