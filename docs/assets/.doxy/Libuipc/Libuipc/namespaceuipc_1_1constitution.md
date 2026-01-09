

# Namespace uipc::constitution



[**Namespace List**](namespaces.md) **>** [**uipc**](namespaceuipc.md) **>** [**constitution**](namespaceuipc_1_1constitution.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**ARAP**](classuipc_1_1constitution_1_1ARAP.md) <br> |
| class | [**AffineBodyConstitution**](classuipc_1_1constitution_1_1AffineBodyConstitution.md) <br> |
| class | [**AffineBodyDrivingRevoluteJoint**](classuipc_1_1constitution_1_1AffineBodyDrivingRevoluteJoint.md) <br> |
| class | [**AffineBodyExternalBodyForce**](classuipc_1_1constitution_1_1AffineBodyExternalBodyForce.md) <br> |
| class | [**AffineBodyMaterial**](classuipc_1_1constitution_1_1AffineBodyMaterial.md) <br> |
| class | [**AffineBodyPrismaticJoint**](classuipc_1_1constitution_1_1AffineBodyPrismaticJoint.md) <br> |
| class | [**AffineBodyRevoluteJoint**](classuipc_1_1constitution_1_1AffineBodyRevoluteJoint.md) <br> |
| class | [**Constraint**](classuipc_1_1constitution_1_1Constraint.md) <br> |
| class | [**DiscreteShellBending**](classuipc_1_1constitution_1_1DiscreteShellBending.md) <br> |
| class | [**ElasticModuli**](classuipc_1_1constitution_1_1ElasticModuli.md) <br> |
| class | [**ElasticModuli2D**](classuipc_1_1constitution_1_1ElasticModuli2D.md) <br> |
| class | [**Empty**](classuipc_1_1constitution_1_1Empty.md) <br> |
| class | [**ExternalArticulationConstraint**](classuipc_1_1constitution_1_1ExternalArticulationConstraint.md) <br>_External articulation constraint for incorporating external kinetic energy into the IPC system._  |
| class | [**FiniteElementConstitution**](classuipc_1_1constitution_1_1FiniteElementConstitution.md) <br> |
| class | [**FiniteElementExtraConstitution**](classuipc_1_1constitution_1_1FiniteElementExtraConstitution.md) <br> |
| class | [**HookeanSpring**](classuipc_1_1constitution_1_1HookeanSpring.md) <br> |
| class | [**IConstitution**](classuipc_1_1constitution_1_1IConstitution.md) <br> |
| class | [**InterAffineBodyConstitution**](classuipc_1_1constitution_1_1InterAffineBodyConstitution.md) <br> |
| class | [**InterPrimitiveConstitution**](classuipc_1_1constitution_1_1InterPrimitiveConstitution.md) <br> |
| class | [**KirchhoffRodBending**](classuipc_1_1constitution_1_1KirchhoffRodBending.md) <br> |
| class | [**LinearMotor**](classuipc_1_1constitution_1_1LinearMotor.md) <br> |
| class | [**NeoHookeanShell**](classuipc_1_1constitution_1_1NeoHookeanShell.md) <br> |
| class | [**Particle**](classuipc_1_1constitution_1_1Particle.md) <br> |
| class | [**RotatingMotor**](classuipc_1_1constitution_1_1RotatingMotor.md) <br> |
| class | [**SoftPositionConstraint**](classuipc_1_1constitution_1_1SoftPositionConstraint.md) <br> |
| class | [**SoftTransformConstraint**](classuipc_1_1constitution_1_1SoftTransformConstraint.md) <br> |
| class | [**SoftVertexStitch**](classuipc_1_1constitution_1_1SoftVertexStitch.md) <br> |
| class | [**StableNeoHookean**](classuipc_1_1constitution_1_1StableNeoHookean.md) <br> |
| class | [**StrainLimitingBaraffWitkinShell**](classuipc_1_1constitution_1_1StrainLimitingBaraffWitkinShell.md) <br> |






















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**EG\_to\_lame**](#function-eg_to_lame) (Float E, Float G, Float & lambda, Float & mu, Float & poisson) <br> |
|  void | [**EG\_to\_lame\_2D**](#function-eg_to_lame_2d) (Float E, Float G, Float & lambda, Float & mu, Float & poisson) <br> |
|  void | [**EG\_to\_poisson**](#function-eg_to_poisson) (Float E, Float G, Float & poisson) <br> |
|  void | [**EP\_to\_lame**](#function-ep_to_lame) (Float E, Float poission, Float & lambda, Float & mu) <br> |
|  void | [**EP\_to\_lame\_2D**](#function-ep_to_lame_2d) (Float E, Float poisson, Float & lambda, Float & mu) <br> |
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



### function EG\_to\_lame\_2D 

```C++
inline void uipc::constitution::EG_to_lame_2D (
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



### function EP\_to\_lame\_2D 

```C++
inline void uipc::constitution::EP_to_lame_2D (
    Float E,
    Float poisson,
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

