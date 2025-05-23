

# Class uipc::Exception



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**Exception**](classuipc_1_1_exception.md)








Inherits the following classes: std::exception


Inherited by the following classes: [uipc::JsonIOError](classuipc_1_1_json_i_o_error.md),  [uipc::core::EngineException](classuipc_1_1core_1_1_engine_exception.md),  [uipc::core::SceneIOError](classuipc_1_1core_1_1_scene_i_o_error.md),  [uipc::geometry::AttributeCollectionError](classuipc_1_1geometry_1_1_attribute_collection_error.md),  [uipc::geometry::AttributeIOError](classuipc_1_1geometry_1_1_attribute_i_o_error.md),  [uipc::geometry::GeometryIOError](classuipc_1_1geometry_1_1_geometry_i_o_error.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Exception**](#function-exception) (const string & msg) <br> |
| virtual const char \* | [**what**](#function-what) () noexcept override const<br> |




























## Public Functions Documentation




### function Exception 

```C++
uipc::Exception::Exception (
    const string & msg
) 
```




<hr>



### function what 

```C++
virtual const char * uipc::Exception::what () noexcept override const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/exception.h`

