

# Class uipc::geometry::AttributeCopy



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**CopyType**](#enum-copytype)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AttributeCopy**](#function-attributecopy) () noexcept<br>_Dst[i] = Src[i]._  |
|  CopyType | [**type**](#function-type) () noexcept const<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md) | [**pair**](#function-pair) (span&lt; const std::pair&lt; SizeT, SizeT &gt; &gt; pairs) noexcept<br>_Dst[Pairs[i].first] = Src[Pairs[i].second]._  |
|  [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md) | [**pull**](#function-pull) (span&lt; const SizeT &gt; mapping) noexcept<br>_Dst[i] = Src[Mapping[i]]._  |
|  [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md) | [**push**](#function-push) (span&lt; const SizeT &gt; mapping) noexcept<br>_Dst[Mapping[i]] = Src[i]._  |
|  [**AttributeCopy**](classuipc_1_1geometry_1_1_attribute_copy.md) | [**range**](#function-range) (SizeT dst\_offset, SizeT src\_offset, SizeT count) noexcept<br>_Dst[dst\_offset + i] = Src[src\_offset + i] $$ i \in [0, count) $$._  |


























## Public Types Documentation




### enum CopyType 

```C++
enum uipc::geometry::AttributeCopy::CopyType {
    None = 0,
    SameDim,
    Range,
    Pull,
    Push,
    Pair
};
```




<hr>
## Public Functions Documentation




### function AttributeCopy 

_Dst[i] = Src[i]._ 
```C++
uipc::geometry::AttributeCopy::AttributeCopy () noexcept
```




<hr>



### function type 

```C++
CopyType uipc::geometry::AttributeCopy::type () noexcept const
```




<hr>
## Public Static Functions Documentation




### function pair 

_Dst[Pairs[i].first] = Src[Pairs[i].second]._ 
```C++
static AttributeCopy uipc::geometry::AttributeCopy::pair (
    span< const std::pair< SizeT, SizeT > > pairs
) noexcept
```




<hr>



### function pull 

_Dst[i] = Src[Mapping[i]]._ 
```C++
static AttributeCopy uipc::geometry::AttributeCopy::pull (
    span< const SizeT > mapping
) noexcept
```




<hr>



### function push 

_Dst[Mapping[i]] = Src[i]._ 
```C++
static AttributeCopy uipc::geometry::AttributeCopy::push (
    span< const SizeT > mapping
) noexcept
```




<hr>



### function range 

_Dst[dst\_offset + i] = Src[src\_offset + i] $$ i \in [0, count) $$._ 
```C++
static AttributeCopy uipc::geometry::AttributeCopy::range (
    SizeT dst_offset,
    SizeT src_offset,
    SizeT count
) noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/attribute_copy.h`

