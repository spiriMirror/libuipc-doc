

# Class uipc::constitution::ElasticModuli2D



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**ElasticModuli2D**](classuipc_1_1constitution_1_1ElasticModuli2D.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  auto | [**lambda**](#function-lambda) () noexcept const<br> |
|  auto | [**mu**](#function-mu) () noexcept const<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**ElasticModuli2D**](classuipc_1_1constitution_1_1ElasticModuli2D.md) | [**lame**](#function-lame) (Float lambda, Float mu) noexcept<br> |
|  [**ElasticModuli2D**](classuipc_1_1constitution_1_1ElasticModuli2D.md) | [**youngs\_poisson**](#function-youngs_poisson) (Float E, Float nu) <br> |
|  [**ElasticModuli2D**](classuipc_1_1constitution_1_1ElasticModuli2D.md) | [**youngs\_shear**](#function-youngs_shear) (Float E, Float G) noexcept<br> |


























## Public Functions Documentation




### function lambda 

```C++
inline auto uipc::constitution::ElasticModuli2D::lambda () noexcept const
```




<hr>



### function mu 

```C++
inline auto uipc::constitution::ElasticModuli2D::mu () noexcept const
```




<hr>
## Public Static Functions Documentation




### function lame 

```C++
static ElasticModuli2D uipc::constitution::ElasticModuli2D::lame (
    Float lambda,
    Float mu
) noexcept
```




<hr>



### function youngs\_poisson 

```C++
static ElasticModuli2D uipc::constitution::ElasticModuli2D::youngs_poisson (
    Float E,
    Float nu
) 
```




<hr>



### function youngs\_shear 

```C++
static ElasticModuli2D uipc::constitution::ElasticModuli2D::youngs_shear (
    Float E,
    Float G
) noexcept
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/elastic_moduli.h`

