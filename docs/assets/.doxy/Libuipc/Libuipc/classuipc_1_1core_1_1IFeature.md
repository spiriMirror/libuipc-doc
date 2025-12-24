

# Class uipc::core::IFeature



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**IFeature**](classuipc_1_1core_1_1IFeature.md)










Inherited by the following classes: [uipc::core::Feature](classuipc_1_1core_1_1Feature.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**name**](#function-name) () const<br> |
|  std::string\_view | [**type\_name**](#function-type_name) () const<br> |
| virtual  | [**~IFeature**](#function-ifeature) () = default<br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**do\_on\_required**](#function-do_on_required) () const = 0<br> |
| virtual std::string\_view | [**get\_name**](#function-get_name) () const = 0<br> |
| virtual std::string\_view | [**get\_type\_name**](#function-get_type_name) () const = 0<br> |




## Public Functions Documentation




### function name 

```C++
std::string_view uipc::core::IFeature::name () const
```




<hr>



### function type\_name 

```C++
std::string_view uipc::core::IFeature::type_name () const
```




<hr>



### function ~IFeature 

```C++
virtual uipc::core::IFeature::~IFeature () = default
```




<hr>
## Protected Functions Documentation




### function do\_on\_required 

```C++
virtual void uipc::core::IFeature::do_on_required () const = 0
```




<hr>



### function get\_name 

```C++
virtual std::string_view uipc::core::IFeature::get_name () const = 0
```




<hr>



### function get\_type\_name 

```C++
virtual std::string_view uipc::core::IFeature::get_type_name () const = 0
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/feature.h`

