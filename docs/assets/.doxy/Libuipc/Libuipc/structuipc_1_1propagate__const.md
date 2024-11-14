

# Struct uipc::propagate\_const

**template &lt;typename T, typename DstT&gt;**



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**propagate\_const**](structuipc_1_1propagate__const.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::conditional\_t&lt; std::is\_const\_v&lt; T &gt;, const DstT\_, DstT\_ &gt; | [**type**](#typedef-type)  <br> |
















































## Public Types Documentation




### typedef type 

```C++
using uipc::propagate_const< T, DstT >::type =  std::conditional_t<std::is_const_v<T>, const DstT_, DstT_>;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/common/type_traits.h`

