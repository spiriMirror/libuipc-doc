

# Class uipc::details::ScopedTimer



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**details**](namespaceuipc_1_1details.md) **>** [**ScopedTimer**](classuipc_1_1details_1_1ScopedTimer.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::chrono::duration&lt; double &gt; | [**Duration**](#typedef-duration)  <br> |
| typedef std::chrono::time\_point&lt; std::chrono::high\_resolution\_clock &gt; | [**TimePoint**](#typedef-timepoint)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**~ScopedTimer**](#function-scopedtimer) () = default<br> |




























## Public Types Documentation




### typedef Duration 

```C++
using uipc::details::ScopedTimer::Duration =  std::chrono::duration<double>;
```




<hr>



### typedef TimePoint 

```C++
using uipc::details::ScopedTimer::TimePoint =  std::chrono::time_point<std::chrono::high_resolution_clock>;
```




<hr>
## Public Functions Documentation




### function ~ScopedTimer 

```C++
uipc::details::ScopedTimer::~ScopedTimer () = default
```




<hr>## Friends Documentation





### friend GlobalTimer 

```C++
class uipc::details::ScopedTimer::GlobalTimer (
    uipc::GlobalTimer
) 
```




<hr>



### friend Timer 

```C++
class uipc::details::ScopedTimer::Timer (
    uipc::Timer
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/timer.h`

