

# Class uipc::core::EngineStatusCollection



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**EngineStatusCollection**](classuipc_1_1core_1_1EngineStatusCollection.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**EngineStatusCollection**](#function-enginestatuscollection) () <br> |
|  void | [**clear**](#function-clear) () <br> |
|  bool | [**has\_error**](#function-has_error) () noexcept const<br> |
|  void | [**push\_back**](#function-push_back-12) (const [**EngineStatus**](classuipc_1_1core_1_1EngineStatus.md) & error) <br> |
|  void | [**push\_back**](#function-push_back-22) ([**EngineStatus**](classuipc_1_1core_1_1EngineStatus.md) && error) <br> |
|  Json | [**to\_json**](#function-to_json) () const<br> |
|   | [**~EngineStatusCollection**](#function-enginestatuscollection) () <br> |




























## Public Functions Documentation




### function EngineStatusCollection 

```C++
uipc::core::EngineStatusCollection::EngineStatusCollection () 
```




<hr>



### function clear 

```C++
void uipc::core::EngineStatusCollection::clear () 
```




<hr>



### function has\_error 

```C++
bool uipc::core::EngineStatusCollection::has_error () noexcept const
```




<hr>



### function push\_back [1/2]

```C++
void uipc::core::EngineStatusCollection::push_back (
    const EngineStatus & error
) 
```




<hr>



### function push\_back [2/2]

```C++
void uipc::core::EngineStatusCollection::push_back (
    EngineStatus && error
) 
```




<hr>



### function to\_json 

```C++
Json uipc::core::EngineStatusCollection::to_json () const
```




<hr>



### function ~EngineStatusCollection 

```C++
uipc::core::EngineStatusCollection::~EngineStatusCollection () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/engine_status.h`

