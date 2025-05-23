

# Class uipc::core::IEngine



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**IEngine**](classuipc_1_1core_1_1_i_engine.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**advance**](#function-advance) () <br> |
|  void | [**backward**](#function-backward) () <br> |
|  bool | [**dump**](#function-dump) () <br> |
|  const [**FeatureCollection**](classuipc_1_1core_1_1_feature_collection.md) & | [**features**](#function-features) () const<br> |
|  SizeT | [**frame**](#function-frame) () const<br> |
|  void | [**init**](#function-init) ([**internal::World**](classuipc_1_1core_1_1internal_1_1_world.md) & w) <br> |
|  bool | [**recover**](#function-recover) (SizeT dst\_frame) <br> |
|  void | [**retrieve**](#function-retrieve) () <br> |
|  [**EngineStatusCollection**](classuipc_1_1core_1_1_engine_status_collection.md) & | [**status**](#function-status) () <br> |
|  void | [**sync**](#function-sync) () <br> |
|  Json | [**to\_json**](#function-to_json) () const<br> |
| virtual  | [**~IEngine**](#function-iengine) () = default<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_advance**](#function-do_advance) () = 0<br> |
| virtual void | [**do\_backward**](#function-do_backward) () = 0<br> |
| virtual bool | [**do\_dump**](#function-do_dump) () <br> |
| virtual void | [**do\_init**](#function-do_init) ([**internal::World**](classuipc_1_1core_1_1internal_1_1_world.md) &) = 0<br> |
| virtual bool | [**do\_recover**](#function-do_recover) (SizeT dst\_frame) <br> |
| virtual void | [**do\_retrieve**](#function-do_retrieve) () = 0<br> |
| virtual void | [**do\_sync**](#function-do_sync) () = 0<br> |
| virtual Json | [**do\_to\_json**](#function-do_to_json) () const<br> |
| virtual const [**FeatureCollection**](classuipc_1_1core_1_1_feature_collection.md) & | [**get\_features**](#function-get_features) () const = 0<br> |
| virtual SizeT | [**get\_frame**](#function-get_frame) () const = 0<br> |
| virtual [**EngineStatusCollection**](classuipc_1_1core_1_1_engine_status_collection.md) & | [**get\_status**](#function-get_status) () = 0<br> |




## Public Functions Documentation




### function advance 

```C++
void uipc::core::IEngine::advance () 
```




<hr>



### function backward 

```C++
void uipc::core::IEngine::backward () 
```




<hr>



### function dump 

```C++
bool uipc::core::IEngine::dump () 
```




<hr>



### function features 

```C++
const FeatureCollection & uipc::core::IEngine::features () const
```




<hr>



### function frame 

```C++
SizeT uipc::core::IEngine::frame () const
```




<hr>



### function init 

```C++
void uipc::core::IEngine::init (
    internal::World & w
) 
```




<hr>



### function recover 

```C++
bool uipc::core::IEngine::recover (
    SizeT dst_frame
) 
```




<hr>



### function retrieve 

```C++
void uipc::core::IEngine::retrieve () 
```




<hr>



### function status 

```C++
EngineStatusCollection & uipc::core::IEngine::status () 
```




<hr>



### function sync 

```C++
void uipc::core::IEngine::sync () 
```




<hr>



### function to\_json 

```C++
Json uipc::core::IEngine::to_json () const
```




<hr>



### function ~IEngine 

```C++
virtual uipc::core::IEngine::~IEngine () = default
```




<hr>
## Protected Functions Documentation




### function do\_advance 

```C++
virtual void uipc::core::IEngine::do_advance () = 0
```




<hr>



### function do\_backward 

```C++
virtual void uipc::core::IEngine::do_backward () = 0
```




<hr>



### function do\_dump 

```C++
virtual bool uipc::core::IEngine::do_dump () 
```




<hr>



### function do\_init 

```C++
virtual void uipc::core::IEngine::do_init (
    internal::World &
) = 0
```




<hr>



### function do\_recover 

```C++
virtual bool uipc::core::IEngine::do_recover (
    SizeT dst_frame
) 
```




<hr>



### function do\_retrieve 

```C++
virtual void uipc::core::IEngine::do_retrieve () = 0
```




<hr>



### function do\_sync 

```C++
virtual void uipc::core::IEngine::do_sync () = 0
```




<hr>



### function do\_to\_json 

```C++
virtual Json uipc::core::IEngine::do_to_json () const
```




<hr>



### function get\_features 

```C++
virtual const FeatureCollection & uipc::core::IEngine::get_features () const = 0
```




<hr>



### function get\_frame 

```C++
virtual SizeT uipc::core::IEngine::get_frame () const = 0
```




<hr>



### function get\_status 

```C++
virtual EngineStatusCollection & uipc::core::IEngine::get_status () = 0
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/i_engine.h`

