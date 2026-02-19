

# Class uipc::constitution::AffineBodyPrismaticJointLimit



[**ClassList**](annotated.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md) **>** [**AffineBodyPrismaticJointLimit**](classuipc_1_1constitution_1_1AffineBodyPrismaticJointLimit.md)








Inherits the following classes: [uipc::constitution::InterAffineBodyExtraConstitution](classuipc_1_1constitution_1_1InterAffineBodyExtraConstitution.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AffineBodyPrismaticJointLimit**](#function-affinebodyprismaticjointlimit) (const Json & config=default\_config()) <br> |
|  void | [**apply\_to**](#function-apply_to-12) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, Float lower, Float upper, Float strength=1.0f) <br> |
|  void | [**apply\_to**](#function-apply_to-22) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc, span&lt; Float &gt; lowers, span&lt; Float &gt; uppers, span&lt; Float &gt; strengths) <br> |
|   | [**~AffineBodyPrismaticJointLimit**](#function-affinebodyprismaticjointlimit) () override<br> |




## Public Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
|  std::string\_view | [**name**](classuipc_1_1constitution_1_1IConstitution.md#function-name) () noexcept const<br> |
|  std::string\_view | [**type**](classuipc_1_1constitution_1_1IConstitution.md#function-type) () noexcept const<br> |
|  U64 | [**uid**](classuipc_1_1constitution_1_1IConstitution.md#function-uid) () noexcept const<br> |
|  const [**builtin::UIDInfo**](structuipc_1_1builtin_1_1UIDInfo.md) & | [**uid\_info**](classuipc_1_1constitution_1_1IConstitution.md#function-uid_info) () noexcept const<br> |
| virtual  | [**~IConstitution**](classuipc_1_1constitution_1_1IConstitution.md#function-iconstitution) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Json | [**default\_config**](#function-default_config) () <br> |




































































## Protected Functions inherited from uipc::constitution::InterAffineBodyExtraConstitution

See [uipc::constitution::InterAffineBodyExtraConstitution](classuipc_1_1constitution_1_1InterAffineBodyExtraConstitution.md)

| Type | Name |
| ---: | :--- |
|  void | [**apply\_to**](classuipc_1_1constitution_1_1InterAffineBodyExtraConstitution.md#function-apply_to) ([**geometry::SimplicialComplex**](classuipc_1_1geometry_1_1SimplicialComplex.md) & sc) const<br> |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1InterAffineBodyExtraConstitution.md#function-get_uid) () noexcept const = 0<br> |


## Protected Functions inherited from uipc::constitution::IConstitution

See [uipc::constitution::IConstitution](classuipc_1_1constitution_1_1IConstitution.md)

| Type | Name |
| ---: | :--- |
| virtual U64 | [**get\_uid**](classuipc_1_1constitution_1_1IConstitution.md#function-get_uid) () noexcept const = 0<br> |








## Public Functions Documentation




### function AffineBodyPrismaticJointLimit 

```C++
uipc::constitution::AffineBodyPrismaticJointLimit::AffineBodyPrismaticJointLimit (
    const Json & config=default_config()
) 
```




<hr>



### function apply\_to [1/2]

```C++
void uipc::constitution::AffineBodyPrismaticJointLimit::apply_to (
    geometry::SimplicialComplex & sc,
    Float lower,
    Float upper,
    Float strength=1.0f
) 
```




<hr>



### function apply\_to [2/2]

```C++
void uipc::constitution::AffineBodyPrismaticJointLimit::apply_to (
    geometry::SimplicialComplex & sc,
    span< Float > lowers,
    span< Float > uppers,
    span< Float > strengths
) 
```




<hr>



### function ~AffineBodyPrismaticJointLimit 

```C++
uipc::constitution::AffineBodyPrismaticJointLimit::~AffineBodyPrismaticJointLimit () override
```




<hr>
## Public Static Functions Documentation




### function default\_config 

```C++
static Json uipc::constitution::AffineBodyPrismaticJointLimit::default_config () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_prismatic_joint_limit.h`

