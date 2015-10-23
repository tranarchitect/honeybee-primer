## ![](../../images/icons/Radiance_Trans_Material_By_Color.png) Radiance Trans Material By Color

![](../../images/components/Radiance_Trans_Material_By_Color.png)

Radiance Trans Material

#### Inputs
* ##### materialName [Required]
Unique name for this material
* ##### color [Required]
Material color
* ##### specularReflection [Required]
Reflected specularity; Matte = min 0, Uncoated Glass ~ .06, Satin = suggested max 0.07
* ##### diffuseTransmission [Required]
Diffuse Transmission; Opaque = 0, Transparent = 1
* ##### specularTransmission [Required]
Specular Transmission; Diffuse = 0, Clear = 1
* ##### roughness [Default]
Specular Transmission; Diffuse = 0, Clear = 1

#### Outputs
* ##### transMaterial
Radiance Material Definition


[Check Hydra Example Files for Radiance Trans Material By Color](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Radiance Trans Material By Color)