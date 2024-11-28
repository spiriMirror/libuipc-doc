

# Class uipc::geometry::SimplicialComplexAttributes

**template &lt;bool IsConst, IndexT N&gt;**



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; IsConst, const [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md), [**AttributeCollection**](classuipc_1_1geometry_1_1_attribute_collection.md) &gt; | [**AutoAttributeCollection**](#typedef-autoattributecollection)  <br> |
| typedef std::conditional\_t&lt; IsScalar, IndexT, Vector&lt; IndexT, N+1 &gt; &gt; | [**TopoValueT**](#typedef-topovaluet)  <br> |






## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  constexpr bool | [**IsScalar**](#variable-isscalar)   = = (N == 0)<br> |














## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SimplicialComplexAttributes**](#function-simplicialcomplexattributes-25) (const [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) & o) = default<br> |
|   | [**SimplicialComplexAttributes**](#function-simplicialcomplexattributes-35) ([**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) && o) = default<br> |
|   | [**SimplicialComplexAttributes**](#function-simplicialcomplexattributes-45) (const [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md)&lt; OtherIsConst, N &gt; & o) noexcept<br> |
|  void | [**clear**](#function-clear) () <br> |
|  void | [**copy\_from**](#function-copy_from) ([**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md)&lt; true, N &gt; other, const [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md) & copy={}, span&lt; const string &gt; include\_names={}, span&lt; const string &gt; exclude\_names={}) <br> |
|  decltype(auto) | [**create**](#function-create) (std::string\_view name, const T & default\_value={}, bool allow\_destroy=true) <br> |
|  void | [**destroy**](#function-destroy) (std::string\_view name) <br> |
|  decltype(auto) | [**find**](#function-find-12) (std::string\_view name) <br>_Find an attribute by type and name, if the attribute does not exist, return nullptr._  |
|  decltype(auto) | [**find**](#function-find-22) (std::string\_view name) const<br>_Find an attribute by type and name, if the attribute does not exist, return nullptr._  |
|  [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) & | [**operator=**](#function-operator) (const [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) & o) = default<br> |
|  [**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) & | [**operator=**](#function-operator_1) ([**SimplicialComplexAttributes**](classuipc_1_1geometry_1_1_simplicial_complex_attributes.md) && o) = default<br> |
|  void | [**reserve**](#function-reserve) (SizeT size) <br> |
|  void | [**resize**](#function-resize) (SizeT size) <br> |
|  decltype(auto) | [**share**](#function-share) (std::string\_view name, const [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; T &gt; & slot, bool allow\_destroy=true) <br> |
|  SizeT | [**size**](#function-size) () noexcept const<br> |
|  Json | [**to\_json**](#function-to_json) () const<br> |
|  [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; TopoValueT &gt; & | [**topo**](#function-topo-12) () <br>_Get the topology of the simplicial complex._  |
|  const [**AttributeSlot**](classuipc_1_1geometry_1_1_attribute_slot.md)&lt; TopoValueT &gt; & | [**topo**](#function-topo-22) () const<br> |




























## Public Types Documentation




### typedef AutoAttributeCollection 

```C++
using uipc::geometry::SimplicialComplexAttributes< IsConst, N >::AutoAttributeCollection = 
        std::conditional_t<IsConst, const AttributeCollection, AttributeCollection>;
```




<hr>



### typedef TopoValueT 

```C++
using uipc::geometry::SimplicialComplexAttributes< IsConst, N >::TopoValueT =  std::conditional_t<IsScalar, IndexT, Vector<IndexT, N + 1>>;
```




<hr>
## Public Static Attributes Documentation




### variable IsScalar 

```C++
constexpr bool uipc::geometry::SimplicialComplexAttributes< IsConst, N >::IsScalar;
```




<hr>
## Public Functions Documentation




### function SimplicialComplexAttributes [2/5]

```C++
uipc::geometry::SimplicialComplexAttributes::SimplicialComplexAttributes (
    const SimplicialComplexAttributes & o
) = default
```




<hr>



### function SimplicialComplexAttributes [3/5]

```C++
uipc::geometry::SimplicialComplexAttributes::SimplicialComplexAttributes (
    SimplicialComplexAttributes && o
) = default
```




<hr>



### function SimplicialComplexAttributes [4/5]

```C++
template<bool OtherIsConst>
inline uipc::geometry::SimplicialComplexAttributes::SimplicialComplexAttributes (
    const SimplicialComplexAttributes < OtherIsConst, N > & o
) noexcept
```




<hr>



### function clear 


```C++
inline void uipc::geometry::SimplicialComplexAttributes::clear () 
```





**See also:** [**AttributeCollection::clear**](classuipc_1_1geometry_1_1_attribute_collection.md#function-clear) 



        

<hr>



### function copy\_from 

```C++
inline void uipc::geometry::SimplicialComplexAttributes::copy_from (
    SimplicialComplexAttributes < true, N > other,
    const AttributeCopy & copy={},
    span< const string > include_names={},
    span< const string > exclude_names={}
) 
```




<hr>



### function create 

```C++
template<typename T>
inline decltype(auto) uipc::geometry::SimplicialComplexAttributes::create (
    std::string_view name,
    const T & default_value={},
    bool allow_destroy=true
) 
```




<hr>



### function destroy 


```C++
inline void uipc::geometry::SimplicialComplexAttributes::destroy (
    std::string_view name
) 
```





**See also:** [**AttributeCollection::destroy**](classuipc_1_1geometry_1_1_attribute_collection.md#function-destroy) 



        

<hr>



### function find [1/2]

```C++
template<typename T>
inline decltype(auto) uipc::geometry::SimplicialComplexAttributes::find (
    std::string_view name
) 
```




<hr>



### function find [2/2]

```C++
template<typename T>
inline decltype(auto) uipc::geometry::SimplicialComplexAttributes::find (
    std::string_view name
) const
```




<hr>



### function operator= 

```C++
SimplicialComplexAttributes & uipc::geometry::SimplicialComplexAttributes::operator= (
    const SimplicialComplexAttributes & o
) = default
```




<hr>



### function operator= 

```C++
SimplicialComplexAttributes & uipc::geometry::SimplicialComplexAttributes::operator= (
    SimplicialComplexAttributes && o
) = default
```




<hr>



### function reserve 


```C++
inline void uipc::geometry::SimplicialComplexAttributes::reserve (
    SizeT size
) 
```





**See also:** [**AttributeCollection::reserve**](classuipc_1_1geometry_1_1_attribute_collection.md#function-reserve) 



        

<hr>



### function resize 


```C++
inline void uipc::geometry::SimplicialComplexAttributes::resize (
    SizeT size
) 
```





**See also:** [**AttributeCollection::resize**](classuipc_1_1geometry_1_1_attribute_collection.md#function-resize) 



        

<hr>



### function share 

```C++
template<typename T>
inline decltype(auto) uipc::geometry::SimplicialComplexAttributes::share (
    std::string_view name,
    const AttributeSlot < T > & slot,
    bool allow_destroy=true
) 
```




<hr>



### function size 


```C++
inline SizeT uipc::geometry::SimplicialComplexAttributes::size () noexcept const
```





**See also:** [**AttributeCollection::size**](classuipc_1_1geometry_1_1_attribute_collection.md#function-size) 



        

<hr>



### function to\_json 

```C++
inline Json uipc::geometry::SimplicialComplexAttributes::to_json () const
```




<hr>



### function topo [1/2]

_Get the topology of the simplicial complex._ 
```C++
inline AttributeSlot < TopoValueT > & uipc::geometry::SimplicialComplexAttributes::topo () 
```





**Returns:**

Topo 





        

<hr>



### function topo [2/2]

```C++
inline const AttributeSlot < TopoValueT > & uipc::geometry::SimplicialComplexAttributes::topo () const
```




<hr>## Friends Documentation





### friend AttributeFriend 

```C++
template<typename T>
class uipc::geometry::SimplicialComplexAttributes::AttributeFriend (
    AttributeFriend
) 
```




<hr>



### friend SimplicialComplexAttributes [1/5]

```C++
template<bool OtherIsConst, IndexT OtherN>
class uipc::geometry::SimplicialComplexAttributes::SimplicialComplexAttributes (
    SimplicialComplexAttributes
) 
```




<hr>



### friend formatter&lt; SimplicialComplexAttributes&lt; IsConst, N &gt; &gt; 

```C++
class uipc::geometry::SimplicialComplexAttributes::formatter< SimplicialComplexAttributes< IsConst, N > > (
    fmt::formatter< SimplicialComplexAttributes < IsConst, N > >
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/simplicial_complex_attributes.h`

