

# Class uipc::geometry::AttributeCollectionFactory



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**AttributeCollectionFactory**](classuipc_1_1geometry_1_1_attribute_collection_factory.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AttributeCollectionFactory**](#function-attributecollectionfactory) () <br> |
|  S&lt; [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**from\_json**](#function-from_json) (const Json & j, span&lt; S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1_i_attribute_slot.md) &gt; &gt; attributes) <br> |
|  Json | [**to\_json**](#function-to_json) (const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) \* acs, unordered\_map&lt; [**IAttribute**](classuipc_1_1geometry_1_1_i_attribute.md) \*, IndexT &gt; attr\_to\_index) <br> |
|   | [**~AttributeCollectionFactory**](#function-attributecollectionfactory) () <br> |




























## Public Functions Documentation




### function AttributeCollectionFactory 

```C++
uipc::geometry::AttributeCollectionFactory::AttributeCollectionFactory () 
```




<hr>



### function from\_json 

```C++
S< AttributeCollection > uipc::geometry::AttributeCollectionFactory::from_json (
    const Json & j,
    span< S< IAttributeSlot > > attributes
) 
```




<hr>



### function to\_json 

```C++
Json uipc::geometry::AttributeCollectionFactory::to_json (
    const AttributeCollection * acs,
    unordered_map< IAttribute *, IndexT > attr_to_index
) 
```




<hr>



### function ~AttributeCollectionFactory 

```C++
uipc::geometry::AttributeCollectionFactory::~AttributeCollectionFactory () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/attribute_collection_factory.h`

