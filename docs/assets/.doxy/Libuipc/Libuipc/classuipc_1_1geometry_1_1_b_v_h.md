

# Class uipc::geometry::BVH



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**geometry**](namespaceuipc_1_1geometry.md) **>** [**BVH**](classuipc_1_1geometry_1_1_b_v_h.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef Eigen::AlignedBox&lt; Float, 3 &gt; | [**AABB**](#typedef-aabb)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**BVH**](#function-bvh) () <br> |
|  void | [**build**](#function-build) (span&lt; const AABB &gt; aabbs) <br>_Build the_ [_**BVH**_](classuipc_1_1geometry_1_1_b_v_h.md) _tree from a list of AABBs._ |
|  void | [**clear**](#function-clear) () <br>_Clear the_ [_**BVH**_](classuipc_1_1geometry_1_1_b_v_h.md) _tree._ |
|  void | [**query**](#function-query) (span&lt; const AABB &gt; aabbs, std::function&lt; void(IndexT, IndexT)&gt; && QF) const<br>_Query the_ [_**BVH**_](classuipc_1_1geometry_1_1_b_v_h.md) _tree with a list of AABBs._ |
|   | [**~BVH**](#function-bvh) () <br> |




























## Public Types Documentation




### typedef AABB 

```C++
using uipc::geometry::BVH::AABB =  Eigen::AlignedBox<Float, 3>;
```




<hr>
## Public Functions Documentation




### function BVH 

```C++
uipc::geometry::BVH::BVH () 
```




<hr>



### function build 

_Build the_ [_**BVH**_](classuipc_1_1geometry_1_1_b_v_h.md) _tree from a list of AABBs._
```C++
void uipc::geometry::BVH::build (
    span< const AABB > aabbs
) 
```





**Parameters:**


* `aabbs` AABBs 




        

<hr>



### function clear 

```C++
void uipc::geometry::BVH::clear () 
```




<hr>



### function query 

_Query the_ [_**BVH**_](classuipc_1_1geometry_1_1_b_v_h.md) _tree with a list of AABBs._
```C++
void uipc::geometry::BVH::query (
    span< const AABB > aabbs,
    std::function< void(IndexT, IndexT)> && QF
) const
```





**Parameters:**


* `aabbs` AABBs 
* `QF` f:void(IndexT, IndexT), where the two indices are the indices of the two AABBs that intersect, the first index is from the input list, and the second index is from the [**BVH**](classuipc_1_1geometry_1_1_b_v_h.md) tree's AABBs. 




        

<hr>



### function ~BVH 

```C++
uipc::geometry::BVH::~BVH () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/geometry/utils/bvh.h`

