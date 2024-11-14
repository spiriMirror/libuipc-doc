

# Class uipc::GlobalTimer



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**GlobalTimer**](classuipc_1_1_global_timer.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GlobalTimer**](#function-globaltimer-12) (std::string\_view name="GlobalTimer") <br> |
|   | [**GlobalTimer**](#function-globaltimer-22) (const [**GlobalTimer**](classuipc_1_1_global_timer.md) &) = delete<br> |
|  void | [**clear**](#function-clear) () <br> |
|  [**GlobalTimer**](classuipc_1_1_global_timer.md) & | [**operator=**](#function-operator) (const [**GlobalTimer**](classuipc_1_1_global_timer.md) &) = delete<br> |
|  void | [**print\_merged\_timings**](#function-print_merged_timings) (std::ostream & o=std::cout) <br> |
|  void | [**print\_timings**](#function-print_timings) (std::ostream & o=std::cout) <br> |
|  Json | [**report\_as\_json**](#function-report_as_json) () <br> |
|  Json | [**report\_merged\_as\_json**](#function-report_merged_as_json) () <br> |
|  void | [**set\_as\_current**](#function-set_as_current) () <br> |
|   | [**~GlobalTimer**](#function-globaltimer) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**GlobalTimer**](classuipc_1_1_global_timer.md) \* | [**current**](#function-current) () <br> |


























## Public Functions Documentation




### function GlobalTimer [1/2]

```C++
uipc::GlobalTimer::GlobalTimer (
    std::string_view name="GlobalTimer"
) 
```




<hr>



### function GlobalTimer [2/2]

```C++
uipc::GlobalTimer::GlobalTimer (
    const GlobalTimer &
) = delete
```




<hr>



### function clear 

```C++
void uipc::GlobalTimer::clear () 
```




<hr>



### function operator= 

```C++
GlobalTimer & uipc::GlobalTimer::operator= (
    const GlobalTimer &
) = delete
```




<hr>



### function print\_merged\_timings 

```C++
void uipc::GlobalTimer::print_merged_timings (
    std::ostream & o=std::cout
) 
```




<hr>



### function print\_timings 

```C++
void uipc::GlobalTimer::print_timings (
    std::ostream & o=std::cout
) 
```




<hr>



### function report\_as\_json 

```C++
Json uipc::GlobalTimer::report_as_json () 
```




<hr>



### function report\_merged\_as\_json 

```C++
Json uipc::GlobalTimer::report_merged_as_json () 
```




<hr>



### function set\_as\_current 

```C++
void uipc::GlobalTimer::set_as_current () 
```




<hr>



### function ~GlobalTimer 

```C++
uipc::GlobalTimer::~GlobalTimer () 
```




<hr>
## Public Static Functions Documentation




### function current 

```C++
static GlobalTimer * uipc::GlobalTimer::current () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/timer.h`

