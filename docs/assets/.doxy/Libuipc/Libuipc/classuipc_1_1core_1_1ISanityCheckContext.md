

# Class uipc::core::ISanityCheckContext



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**ISanityCheckContext**](classuipc_1_1core_1_1ISanityCheckContext.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual const [**geometry::AttributeCollection**](classuipc_1_1geometry_1_1AttributeCollection.md) & | [**config**](#function-config) () const = 0<br> |
| virtual const [**ContactTabular**](classuipc_1_1core_1_1ContactTabular.md) & | [**contact\_tabular**](#function-contact_tabular) () const = 0<br> |
| virtual S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &gt; | [**find\_geometry**](#function-find_geometry) (IndexT id) const = 0<br> |
| virtual S&lt; const [**Object**](classuipc_1_1core_1_1Object.md) &gt; | [**find\_object**](#function-find_object) (IndexT id) const = 0<br> |
| virtual span&lt; S&lt; [**geometry::GeometrySlot**](classuipc_1_1geometry_1_1GeometrySlot.md) &gt; &gt; | [**geometries**](#function-geometries) () const = 0<br> |
| virtual const [**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & | [**scene\_simplicial\_surface**](#function-scene_simplicial_surface) () const = 0<br> |
| virtual const [**SubsceneTabular**](classuipc_1_1core_1_1SubsceneTabular.md) & | [**subscene\_tabular**](#function-subscene_tabular) () const = 0<br> |
| virtual std::string\_view | [**workspace**](#function-workspace) () const = 0<br> |
| virtual  | [**~ISanityCheckContext**](#function-isanitycheckcontext) () = default<br> |




























## Public Functions Documentation




### function config 

```C++
virtual const geometry::AttributeCollection & uipc::core::ISanityCheckContext::config () const = 0
```




<hr>



### function contact\_tabular 

```C++
virtual const ContactTabular & uipc::core::ISanityCheckContext::contact_tabular () const = 0
```




<hr>



### function find\_geometry 

```C++
virtual S< geometry::GeometrySlot > uipc::core::ISanityCheckContext::find_geometry (
    IndexT id
) const = 0
```




<hr>



### function find\_object 

```C++
virtual S< const Object > uipc::core::ISanityCheckContext::find_object (
    IndexT id
) const = 0
```




<hr>



### function geometries 

```C++
virtual span< S< geometry::GeometrySlot > > uipc::core::ISanityCheckContext::geometries () const = 0
```




<hr>



### function scene\_simplicial\_surface 

```C++
virtual const geometry::SimplicialComplex & uipc::core::ISanityCheckContext::scene_simplicial_surface () const = 0
```




<hr>



### function subscene\_tabular 

```C++
virtual const SubsceneTabular & uipc::core::ISanityCheckContext::subscene_tabular () const = 0
```




<hr>



### function workspace 

```C++
virtual std::string_view uipc::core::ISanityCheckContext::workspace () const = 0
```




<hr>



### function ~ISanityCheckContext 

```C++
virtual uipc::core::ISanityCheckContext::~ISanityCheckContext () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/i_sanity_checker.h`

