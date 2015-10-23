## ![](../../images/icons/Create_EP_Ground.png) Create EP Ground

![](../../images/components/Create_EP_Ground.png)

Use this component to change the properties of a zone to refelct those of a ground.  This is particularly useful for setting up outdoor thermal comfort maps when you want the surface temperature of the ground to be caclated with some spatial diversity, reflecting the shadows that other objects cast upon it and the storage of heat in the ground surface.

#### Inputs
* ##### HBZones [Required]
HBZones to be turned into ground zones, representative of soil.
* ##### soilTypeOrMat [Required]
Either a material definition output from the 'Honeybee_EnergyPlus Opaque Material' component, the name of a material already in the library, or an integer from 0 to 6 representing the following:

#### Outputs
* ##### HBGrndZones
HBZones that have had their properties altered to be ground conditions.


[Check Hydra Example Files for Create EP Ground](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Create EP Ground)