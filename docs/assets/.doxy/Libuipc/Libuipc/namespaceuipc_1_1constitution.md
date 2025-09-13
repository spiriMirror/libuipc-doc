

# Namespace uipc::constitution



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**ARAP**](classuipc_1_1constitution_1_1_a_r_a_p.md) <br> |
| class | [**AffineBodyConstitution**](classuipc_1_1constitution_1_1_affine_body_constitution.md) <br> |
| class | [**AffineBodyDrivingRevoluteJoint**](classuipc_1_1constitution_1_1_affine_body_driving_revolute_joint.md) <br> |
| class | [**AffineBodyMaterial**](classuipc_1_1constitution_1_1_affine_body_material.md) <br> |
| class | [**AffineBodyRevoluteJoint**](classuipc_1_1constitution_1_1_affine_body_revolute_joint.md) <br> |
| class | [**Constraint**](classuipc_1_1constitution_1_1_constraint.md) <br> |
| class | [**DiscreteShellBending**](classuipc_1_1constitution_1_1_discrete_shell_bending.md) <br> |
| class | [**ElasticModuli**](classuipc_1_1constitution_1_1_elastic_moduli.md) <br> |
| class | [**Empty**](classuipc_1_1constitution_1_1_empty.md) <br> |
| class | [**FiniteElementConstitution**](classuipc_1_1constitution_1_1_finite_element_constitution.md) <br> |
| class | [**FiniteElementExtraConstitution**](classuipc_1_1constitution_1_1_finite_element_extra_constitution.md) <br> |
| class | [**HookeanSpring**](classuipc_1_1constitution_1_1_hookean_spring.md) <br> |
| class | [**IConstitution**](classuipc_1_1constitution_1_1_i_constitution.md) <br> |
| class | [**InterAffineBodyConstitution**](classuipc_1_1constitution_1_1_inter_affine_body_constitution.md) <br> |
| class | [**InterPrimitiveConstitution**](classuipc_1_1constitution_1_1_inter_primitive_constitution.md) <br> |
| class | [**KirchhoffRodBending**](classuipc_1_1constitution_1_1_kirchhoff_rod_bending.md) <br> |
| class | [**LinearMotor**](classuipc_1_1constitution_1_1_linear_motor.md) <br> |
| class | [**NeoHookeanShell**](classuipc_1_1constitution_1_1_neo_hookean_shell.md) <br> |
| class | [**Particle**](classuipc_1_1constitution_1_1_particle.md) <br> |
| class | [**RotatingMotor**](classuipc_1_1constitution_1_1_rotating_motor.md) <br> |
| class | [**SoftPositionConstraint**](classuipc_1_1constitution_1_1_soft_position_constraint.md) <br> |
| class | [**SoftTransformConstraint**](classuipc_1_1constitution_1_1_soft_transform_constraint.md) <br> |
| class | [**SoftVertexStitch**](classuipc_1_1constitution_1_1_soft_vertex_stitch.md) <br> |
| class | [**StableNeoHookean**](classuipc_1_1constitution_1_1_stable_neo_hookean.md) <br> |
| class | [**StrainLimitingBaraffWitkinShell**](classuipc_1_1constitution_1_1_strain_limiting_baraff_witkin_shell.md) <br> |






















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**EG\_to\_lame**](#function-eg_to_lame) (Float E, Float G, Float & lambda, Float & mu, Float & poisson) <br> |
|  void | [**EG\_to\_poisson**](#function-eg_to_poisson) (Float E, Float G, Float & poisson) <br> |
|  void | [**EP\_to\_lame**](#function-ep_to_lame) (Float E, Float poission, Float & lambda, Float & mu) <br> |
|  void | [**lame\_to\_EG**](#function-lame_to_eg) (Float lambda, Float mu, Float & E, Float & G, Float & poisson) <br> |
|  void | [**lame\_to\_poisson**](#function-lame_to_poisson) (Float lambda, Float mu, Float & poisson) <br> |




























## Public Functions Documentation




### function EG\_to\_lame 

```C++
inline void uipc::constitution::EG_to_lame (
    Float E,
    Float G,
    Float & lambda,
    Float & mu,
    Float & poisson
) 
```




<hr>



### function EG\_to\_poisson 

```C++
inline void uipc::constitution::EG_to_poisson (
    Float E,
    Float G,
    Float & poisson
) 
```




<hr>



### function EP\_to\_lame 

```C++
inline void uipc::constitution::EP_to_lame (
    Float E,
    Float poission,
    Float & lambda,
    Float & mu
) 
```




<hr>



### function lame\_to\_EG 

```C++
inline void uipc::constitution::lame_to_EG (
    Float lambda,
    Float mu,
    Float & E,
    Float & G,
    Float & poisson
) 
```




<hr>



### function lame\_to\_poisson 

```C++
inline void uipc::constitution::lame_to_poisson (
    Float lambda,
    Float mu,
    Float & poisson
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `include/uipc/constitution/affine_body_constitution.h`

