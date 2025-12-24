

# Class uipc::Timer



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**Timer**](classuipc_1_1Timer.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Timer**](#function-timer) (std::string\_view blockName, bool force\_on=false) <br> |
|  double | [**elapsed**](#function-elapsed) () const<br> |
|   | [**~Timer**](#function-timer) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**disable\_all**](#function-disable_all) () <br> |
|  void | [**enable\_all**](#function-enable_all) () <br> |
|  void | [**report**](#function-report) (std::ostream & o=std::cout) <br> |
|  Json | [**report\_as\_json**](#function-report_as_json) () <br> |
|  void | [**set\_sync\_func**](#function-set_sync_func) (std::function&lt; void()&gt; sync) <br> |


























## Public Functions Documentation




### function Timer 

```C++
uipc::Timer::Timer (
    std::string_view blockName,
    bool force_on=false
) 
```




<hr>



### function elapsed 

```C++
double uipc::Timer::elapsed () const
```




<hr>



### function ~Timer 

```C++
uipc::Timer::~Timer () 
```




<hr>
## Public Static Functions Documentation




### function disable\_all 

```C++
static inline void uipc::Timer::disable_all () 
```




<hr>



### function enable\_all 

```C++
static inline void uipc::Timer::enable_all () 
```




<hr>



### function report 

```C++
static void uipc::Timer::report (
    std::ostream & o=std::cout
) 
```




<hr>



### function report\_as\_json 

```C++
static Json uipc::Timer::report_as_json () 
```




<hr>



### function set\_sync\_func 

```C++
static inline void uipc::Timer::set_sync_func (
    std::function< void()> sync
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/timer.h`

