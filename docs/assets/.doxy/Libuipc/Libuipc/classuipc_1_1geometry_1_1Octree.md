

# Class uipc::geometry::Octree



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**Octree**](classuipc_1_1geometry_1_1Octree.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::AlignedBox&lt; Float, 3 &gt; | [**AABB**](#typedef-aabb)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Octree**](#function-octree) () <br> |
|  void | [**build**](#function-build) (span&lt; const AABB &gt; aabbs) <br>_Build the octree from a list of AABBs._  |
|  void | [**clear**](#function-clear) () <br>_Clear the octree._  |
|  void | [**detect**](#function-detect) (std::function&lt; void(IndexT, IndexT)&gt; && QF) const<br>_Detect the self-intersections of the octree._  |
|  void | [**query**](#function-query) (span&lt; const AABB &gt; aabbs, std::function&lt; void(IndexT, IndexT)&gt; && QF) const<br>_Query the octree with a list of AABBs._  |
|   | [**~Octree**](#function-octree) () <br> |




























## Public Types Documentation




### typedef AABB 

```C++
using uipc::geometry::Octree::AABB =  Eigen::AlignedBox<Float, 3>;
```




<hr>
## Public Functions Documentation




### function Octree 

```C++
uipc::geometry::Octree::Octree () 
```




<hr>



### function build 

_Build the octree from a list of AABBs._ 
```C++
void uipc::geometry::Octree::build (
    span< const AABB > aabbs
) 
```





**Parameters:**


* `aabbs` AABBs 




        

<hr>



### function clear 

_Clear the octree._ 
```C++
void uipc::geometry::Octree::clear () 
```




<hr>



### function detect 

_Detect the self-intersections of the octree._ 
```C++
void uipc::geometry::Octree::detect (
    std::function< void(IndexT, IndexT)> && QF
) const
```





**Parameters:**


* `QF` f:void(IndexT, IndexT), where the two indices are the indices of the two AABBs that intersect, the two indices are from the octree's AABBs. 




        

<hr>



### function query 

_Query the octree with a list of AABBs._ 
```C++
void uipc::geometry::Octree::query (
    span< const AABB > aabbs,
    std::function< void(IndexT, IndexT)> && QF
) const
```





**Parameters:**


* `aabbs` AABBs 
* `QF` f:void(IndexT, IndexT), where the two indices are the indices of the two AABBs that intersect, the first index is from the input list, and the second index is from the octree's AABBs. 




        

<hr>



### function ~Octree 

```C++
uipc::geometry::Octree::~Octree () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/utils/octree.h`

