

# Class uipc::geometry::AttributeCollectionFactory



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**AttributeCollectionFactory**](classuipc_1_1geometry_1_1_attribute_collection_factory.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AttributeCollectionFactory**](#function-attributecollectionfactory) () <br> |
|  S&lt; [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1_attribute_collection_commit.md) &gt; | [**commit\_from\_json**](#function-commit_from_json) (const Json & j, [**DeserialSharedAttributeContext**](classuipc_1_1geometry_1_1_deserial_shared_attribute_context.md) & ctx) <br> |
|  Json | [**commit\_to\_json**](#function-commit_to_json) (const [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1_attribute_collection_commit.md) & acc, [**SerialSharedAttributeContext**](classuipc_1_1geometry_1_1_serial_shared_attribute_context.md) & ctx) <br> |
|  [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1_attribute_collection_commit.md) | [**diff**](#function-diff) (const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) & current, const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) & reference) <br>_Get the difference between the current and reference attribute collections._  |
|  S&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**from\_json**](#function-from_json) (const Json & j, [**DeserialSharedAttributeContext**](classuipc_1_1geometry_1_1_deserial_shared_attribute_context.md) & ctx) <br>_Create an attribute collection from a json object and a pool of shared attributes._  |
|  Json | [**to\_json**](#function-to_json) (const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) & ac, [**SerialSharedAttributeContext**](classuipc_1_1geometry_1_1_serial_shared_attribute_context.md) & ctx) <br> |
|   | [**~AttributeCollectionFactory**](#function-attributecollectionfactory) () <br> |




























## Public Functions Documentation




### function AttributeCollectionFactory 

```C++
uipc::geometry::AttributeCollectionFactory::AttributeCollectionFactory () 
```




<hr>



### function commit\_from\_json 

```C++
S< AttributeCollectionCommit > uipc::geometry::AttributeCollectionFactory::commit_from_json (
    const Json & j,
    DeserialSharedAttributeContext & ctx
) 
```




<hr>



### function commit\_to\_json 

```C++
Json uipc::geometry::AttributeCollectionFactory::commit_to_json (
    const AttributeCollectionCommit & acc,
    SerialSharedAttributeContext & ctx
) 
```




<hr>



### function diff 

_Get the difference between the current and reference attribute collections._ 
```C++
AttributeCollectionCommit uipc::geometry::AttributeCollectionFactory::diff (
    const AttributeCollection & current,
    const AttributeCollection & reference
) 
```




* New Attributes and Modified Attributes will be copied to the diff\_copy.
* Deleted Attributes will be collected in the removed\_names. 




        

<hr>



### function from\_json 

_Create an attribute collection from a json object and a pool of shared attributes._ 
```C++
S< AttributeCollection > uipc::geometry::AttributeCollectionFactory::from_json (
    const Json & j,
    DeserialSharedAttributeContext & ctx
) 
```




<hr>



### function to\_json 

```C++
Json uipc::geometry::AttributeCollectionFactory::to_json (
    const AttributeCollection & ac,
    SerialSharedAttributeContext & ctx
) 
```



@breif Convert an attribute collection to a json object, while using index to replace the attributes pointer 


        

<hr>



### function ~AttributeCollectionFactory 

```C++
uipc::geometry::AttributeCollectionFactory::~AttributeCollectionFactory () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/attribute_collection_factory.h`

