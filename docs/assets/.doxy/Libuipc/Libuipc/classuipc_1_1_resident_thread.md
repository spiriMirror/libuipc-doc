

# Class uipc::ResidentThread



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**ResidentThread**](classuipc_1_1_resident_thread.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**ResidentThread**](#function-residentthread) () <br> |
|  SizeT | [**hash**](#function-hash) () const<br> |
|  bool | [**is\_ready**](#function-is_ready) () const<br> |
|  bool | [**post**](#function-post) (std::function&lt; void()&gt; task) <br> |
|   | [**~ResidentThread**](#function-residentthread) () <br> |




























## Public Functions Documentation




### function ResidentThread 

```C++
uipc::ResidentThread::ResidentThread () 
```




<hr>



### function hash 

```C++
SizeT uipc::ResidentThread::hash () const
```




<hr>



### function is\_ready 

```C++
bool uipc::ResidentThread::is_ready () const
```




<hr>



### function post 

```C++
bool uipc::ResidentThread::post (
    std::function< void()> task
) 
```




<hr>



### function ~ResidentThread 

```C++
uipc::ResidentThread::~ResidentThread () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/resident_thread.h`

