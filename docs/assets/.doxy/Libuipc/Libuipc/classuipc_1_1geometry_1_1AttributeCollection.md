

# Class uipc::geometry::AttributeCollection



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md)



_A collection of geometries attributes._ [More...](#detailed-description)

* `#include <attribute_collection.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AttributeCollection**](#function-attributecollection-13) () = default<br> |
|   | [**AttributeCollection**](#function-attributecollection-23) (const [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) &) <br> |
|   | [**AttributeCollection**](#function-attributecollection-33) ([**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) &&) noexcept<br> |
|  SizeT | [**attribute\_count**](#function-attribute_count) () const<br>_Get the number of attribute slots._  |
|  void | [**clear**](#function-clear) () <br>_clear the underlying attribute values of all attribute slots, the attribute slots will not be destroyed._  |
|  void | [**copy\_from**](#function-copy_from) (const [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) & other, const [**AttributeCopy**](classuipc_1_1geometry_1_1AttributeCopy.md) & copy, span&lt; const string &gt; include\_names={}, span&lt; const string &gt; exclude\_names={}) <br>_copy\_from the underlying attribute values of all attribute slots._  |
|  S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; T &gt; &gt; | [**create**](#function-create) (std::string\_view name, const T & default\_value={}, bool allow\_destroy=true) <br>_Create a new attribute slot of type T with a given name._  |
|  void | [**destroy**](#function-destroy) (std::string\_view name) <br>_Remove the attribute slot with the given name._  |
|  S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1IAttributeSlot.md) &gt; | [**find**](#function-find-14) (std::string\_view name) <br>_Find the attribute slot with the given name._  |
|  S&lt; const [**IAttributeSlot**](classuipc_1_1geometry_1_1IAttributeSlot.md) &gt; | [**find**](#function-find-24) (std::string\_view name) const<br>_const version of find._  |
|  S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; T &gt; &gt; | [**find**](#function-find-34) (std::string\_view name) <br>_Template version of find._  |
|  S&lt; const [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; T &gt; &gt; | [**find**](#function-find-44) (std::string\_view name) const<br>_Template const version of find._  |
|  vector&lt; string &gt; | [**names**](#function-names) () const<br>_Get the names of all attribute slots._  |
|  [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) & | [**operator=**](#function-operator) (const [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) &) <br> |
|  [**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) & | [**operator=**](#function-operator_1) ([**AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) &&) noexcept<br> |
|  void | [**reorder**](#function-reorder) (span&lt; const SizeT &gt; O) <br>_Reorder the underlying attribute values of all attribute slots._  |
|  void | [**reserve**](#function-reserve) (SizeT N) <br>_Reserve memory for all attribute slots._  |
|  void | [**resize**](#function-resize) (SizeT N) <br>_Resize all attribute slots to the given size._  |
|  S&lt; [**IAttributeSlot**](classuipc_1_1geometry_1_1IAttributeSlot.md) &gt; | [**share**](#function-share-12) (std::string\_view name, const [**IAttributeSlot**](classuipc_1_1geometry_1_1IAttributeSlot.md) & slot, bool allow\_destroy=true) <br>_Share the underlying attribute of the given slot with a new name._  |
|  S&lt; [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; T &gt; &gt; | [**share**](#function-share-22) (std::string\_view name, const [**AttributeSlot**](classuipc_1_1geometry_1_1AttributeSlot.md)&lt; T &gt; & slot, bool allow\_destroy=true) <br>_Template version of share._  |
|  SizeT | [**size**](#function-size) () const<br>_Get the size of the attribute slots._  |
|  Json | [**to\_json**](#function-to_json) () const<br>_Get the json representation of the attribute collection._  |
|  void | [**update\_from**](#function-update_from) (const [**AttributeCollectionCommit**](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) & commit) <br>_Update the attribute collection from_ [_**AttributeCollectionCommit**_](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) _._ |




























## Detailed Description


All geometries attributes in the collection always have the same size. 


    
## Public Functions Documentation




### function AttributeCollection [1/3]

```C++
uipc::geometry::AttributeCollection::AttributeCollection () = default
```




<hr>



### function AttributeCollection [2/3]

```C++
uipc::geometry::AttributeCollection::AttributeCollection (
    const AttributeCollection &
) 
```




<hr>



### function AttributeCollection [3/3]

```C++
uipc::geometry::AttributeCollection::AttributeCollection (
    AttributeCollection &&
) noexcept
```




<hr>



### function attribute\_count 

_Get the number of attribute slots._ 
```C++
SizeT uipc::geometry::AttributeCollection::attribute_count () const
```




<hr>



### function clear 

_clear the underlying attribute values of all attribute slots, the attribute slots will not be destroyed._ 
```C++
void uipc::geometry::AttributeCollection::clear () 
```





**Note:**

This method may generate data clones. 





        

<hr>



### function copy\_from 

_copy\_from the underlying attribute values of all attribute slots._ 
```C++
void uipc::geometry::AttributeCollection::copy_from (
    const AttributeCollection & other,
    const AttributeCopy & copy,
    span< const string > include_names={},
    span< const string > exclude_names={}
) 
```





**Parameters:**


* `copy` The copy strategy. 
* `include_names` The names of the attribute slots to be copied. If it is empty, all attribute slots will be copied. 
* `exclude_names` The names of the attribute slots not to be copied, the exclude\_names has higher priority than include\_names. 




        

<hr>



### function create 

_Create a new attribute slot of type T with a given name._ 
```C++
template<typename T>
S< AttributeSlot < T > > uipc::geometry::AttributeCollection::create (
    std::string_view name,
    const T & default_value={},
    bool allow_destroy=true
) 
```





**Template parameters:**


* `T` The type of the attribute values. 



**Parameters:**


* `name` The name of the attribute slot. 



**Returns:**

The created attribute slot. 





        

<hr>



### function destroy 

_Remove the attribute slot with the given name._ 
```C++
void uipc::geometry::AttributeCollection::destroy (
    std::string_view name
) 
```



The underlying attribute will not be destroyed if it is shared by other attribute slots.


@danger Accessing the removed attribute slot will cause undefined behavior. It's user's responsibility to ensure that the removed attribute slot is not accessed. 

**Parameters:**


* `name` 




        

<hr>



### function find [1/4]

_Find the attribute slot with the given name._ 
```C++
S< IAttributeSlot > uipc::geometry::AttributeCollection::find (
    std::string_view name
) 
```





**Parameters:**


* `name` The name of the attribute slot. 



**Returns:**

The attribute slot with the given name. 




**Returns:**

nullptr if the attribute slot with the given name does not exist. 





        

<hr>



### function find [2/4]

_const version of find._ 
```C++
S< const IAttributeSlot > uipc::geometry::AttributeCollection::find (
    std::string_view name
) const
```




<hr>



### function find [3/4]

_Template version of find._ 
```C++
template<typename T>
S< AttributeSlot < T > > uipc::geometry::AttributeCollection::find (
    std::string_view name
) 
```




<hr>



### function find [4/4]

_Template const version of find._ 
```C++
template<typename T>
S< const AttributeSlot < T > > uipc::geometry::AttributeCollection::find (
    std::string_view name
) const
```




<hr>



### function names 

_Get the names of all attribute slots._ 
```C++
vector< string > uipc::geometry::AttributeCollection::names () const
```




<hr>



### function operator= 

```C++
AttributeCollection & uipc::geometry::AttributeCollection::operator= (
    const AttributeCollection &
) 
```




<hr>



### function operator= 

```C++
AttributeCollection & uipc::geometry::AttributeCollection::operator= (
    AttributeCollection &&
) noexcept
```




<hr>



### function reorder 

_Reorder the underlying attribute values of all attribute slots._ 
```C++
void uipc::geometry::AttributeCollection::reorder (
    span< const SizeT > O
) 
```





**Parameters:**


* `O` A New2Old mapping. O[i] = j means the i-th element in the new order has the value of the j-th element in the old order.



**Note:**

This method may generate data clones. 





        

<hr>



### function reserve 

_Reserve memory for all attribute slots._ 
```C++
void uipc::geometry::AttributeCollection::reserve (
    SizeT N
) 
```





**Note:**

This method generates no data clone. But the memory of the underlying attribute values may be reallocated. 





        

<hr>



### function resize 

_Resize all attribute slots to the given size._ 
```C++
void uipc::geometry::AttributeCollection::resize (
    SizeT N
) 
```





**Note:**

This method may generate data clones. 





        

<hr>



### function share [1/2]

_Share the underlying attribute of the given slot with a new name._ 
```C++
S< IAttributeSlot > uipc::geometry::AttributeCollection::share (
    std::string_view name,
    const IAttributeSlot & slot,
    bool allow_destroy=true
) 
```



The slot may be from another geometries attribute collection or just current geometries attribute collection. 

**Parameters:**


* `name` The name of the attribute slot. 
* `slot` The slot brings the underlying attribute. 



**Returns:**

The new created attribute slot.




**Exception:**


* `AttributeAlreadyExist` if the attribute with the given name already exists. 




        

<hr>



### function share [2/2]

_Template version of share._ 
```C++
template<typename T>
S< AttributeSlot < T > > uipc::geometry::AttributeCollection::share (
    std::string_view name,
    const AttributeSlot < T > & slot,
    bool allow_destroy=true
) 
```




<hr>



### function size 

_Get the size of the attribute slots._ 
```C++
SizeT uipc::geometry::AttributeCollection::size () const
```




<hr>



### function to\_json 

_Get the json representation of the attribute collection._ 
```C++
Json uipc::geometry::AttributeCollection::to_json () const
```




<hr>



### function update\_from 

_Update the attribute collection from_ [_**AttributeCollectionCommit**_](classuipc_1_1geometry_1_1AttributeCollectionCommit.md) _._
```C++
void uipc::geometry::AttributeCollection::update_from (
    const AttributeCollectionCommit & commit
) 
```





**Parameters:**


* `commit` 




        

<hr>## Friends Documentation





### friend formatter&lt; AttributeCollection &gt; 

```C++
struct uipc::geometry::AttributeCollection::formatter< AttributeCollection > (
    fmt::formatter< AttributeCollection >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/attribute_collection.h`

