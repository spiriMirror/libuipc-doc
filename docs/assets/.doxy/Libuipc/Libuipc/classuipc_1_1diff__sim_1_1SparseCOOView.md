

# Class uipc::diff\_sim::SparseCOOView



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**diff\_sim**](namespaceuipc_1_1diff__sim.md) **>** [**SparseCOOView**](classuipc_1_1diff__sim_1_1SparseCOOView.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**SparseCOOView**](#function-sparsecooview-12) () = default<br> |
|   | [**SparseCOOView**](#function-sparsecooview-22) (span&lt; const IndexT &gt; row\_indices, span&lt; const IndexT &gt; col\_indices, span&lt; const Float &gt; values, Vector2i shape) <br> |
|  span&lt; const IndexT &gt; | [**col\_indices**](#function-col_indices) () const<br> |
|  span&lt; const IndexT &gt; | [**row\_indices**](#function-row_indices) () const<br> |
|  Vector2i | [**shape**](#function-shape) () const<br> |
|  Matrix&lt; Float, Eigen::Dynamic, Eigen::Dynamic &gt; | [**to\_dense**](#function-to_dense) () const<br> |
|  Eigen::SparseMatrix&lt; Float &gt; | [**to\_sparse**](#function-to_sparse) () const<br> |
|  span&lt; const Float &gt; | [**values**](#function-values) () const<br> |




























## Public Functions Documentation




### function SparseCOOView [1/2]

```C++
uipc::diff_sim::SparseCOOView::SparseCOOView () = default
```




<hr>



### function SparseCOOView [2/2]

```C++
uipc::diff_sim::SparseCOOView::SparseCOOView (
    span< const IndexT > row_indices,
    span< const IndexT > col_indices,
    span< const Float > values,
    Vector2i shape
) 
```




<hr>



### function col\_indices 

```C++
span< const IndexT > uipc::diff_sim::SparseCOOView::col_indices () const
```




<hr>



### function row\_indices 

```C++
span< const IndexT > uipc::diff_sim::SparseCOOView::row_indices () const
```




<hr>



### function shape 

```C++
Vector2i uipc::diff_sim::SparseCOOView::shape () const
```




<hr>



### function to\_dense 

```C++
Matrix< Float, Eigen::Dynamic, Eigen::Dynamic > uipc::diff_sim::SparseCOOView::to_dense () const
```




<hr>



### function to\_sparse 

```C++
Eigen::SparseMatrix< Float > uipc::diff_sim::SparseCOOView::to_sparse () const
```




<hr>



### function values 

```C++
span< const Float > uipc::diff_sim::SparseCOOView::values () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/diff_sim/sparse_coo_view.h`

