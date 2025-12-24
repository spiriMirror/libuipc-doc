

# Class uipc::core::FeatureCollection



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**core**](namespaceuipc_1_1core.md) **>** [**FeatureCollection**](classuipc_1_1core_1_1FeatureCollection.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  bool | [**contains**](#function-contains-12) (std::string\_view name) const<br> |
|  bool | [**contains**](#function-contains-22) () const<br> |
|  S&lt; [**IFeature**](classuipc_1_1core_1_1IFeature.md) &gt; | [**find**](#function-find-12) (std::string\_view name) const<br> |
|  S&lt; T &gt; | [**find**](#function-find-22) (std::string\_view name=T::FeatureName) const<br> |
|  void | [**insert**](#function-insert-12) (std::string\_view name, S&lt; [**IFeature**](classuipc_1_1core_1_1IFeature.md) &gt; feature) <br> |
|  void | [**insert**](#function-insert-22) (S&lt; T &gt; feature) <br> |
|  Json | [**to\_json**](#function-to_json) () const<br> |
| virtual  | [**~FeatureCollection**](#function-featurecollection) () = default<br> |




























## Public Functions Documentation




### function contains [1/2]

```C++
bool uipc::core::FeatureCollection::contains (
    std::string_view name
) const
```




<hr>



### function contains [2/2]

```C++
template<std::derived_from< IFeature > T>
inline bool uipc::core::FeatureCollection::contains () const
```




<hr>



### function find [1/2]

```C++
S< IFeature > uipc::core::FeatureCollection::find (
    std::string_view name
) const
```




<hr>



### function find [2/2]

```C++
template<std::derived_from< IFeature > T>
inline S< T > uipc::core::FeatureCollection::find (
    std::string_view name=T::FeatureName
) const
```




<hr>



### function insert [1/2]

```C++
void uipc::core::FeatureCollection::insert (
    std::string_view name,
    S< IFeature > feature
) 
```




<hr>



### function insert [2/2]

```C++
template<std::derived_from< IFeature > T>
inline void uipc::core::FeatureCollection::insert (
    S< T > feature
) 
```




<hr>



### function to\_json 

```C++
Json uipc::core::FeatureCollection::to_json () const
```




<hr>



### function ~FeatureCollection 

```C++
virtual uipc::core::FeatureCollection::~FeatureCollection () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/core/feature_collection.h`

