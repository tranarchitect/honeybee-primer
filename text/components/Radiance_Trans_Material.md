## ![](../../images/icons/Radiance_Trans_Material.png) Radiance Trans Material

![](../../images/components/Radiance_Trans_Material.png)

Radiance Trans Material

#### Inputs
* ##### materialName [Required]
Unique name for this material
* ##### RDiffReflectance [Required]
Script variable _RDiffReflectance
* ##### GDiffReflectance [Required]
Script variable _GDiffReflectance
* ##### BDiffReflectance [Required]
Script variable _BDiffReflectance
* ##### specularReflection [Required]
Reflected specularity; Matte = min 0, Uncoated Glass ~ .06, Satin = suggested max 0.07
* ##### diffuseTransmission [Required]
Diffuse Transmission; Opaque = 0, Transparent = 1
* ##### specularTransmission [Required]
Specular Transmission; Diffuse = 0, Clear = 1
* ##### roughness [Default]
Surface roughness; Polished = 0, Low gloss = suggested max 0.02

#### Outputs
* ##### transMaterial
Radiance Material Definition


[Check Hydra Example Files for Radiance Trans Material](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Radiance Trans Material)