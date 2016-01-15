## ![](../../images/icons/IES_Luminaire_Zone.png) IES Luminaire Zone

![](../../images/components/IES_Luminaire_Zone.png)

    This component is to be used for specifying the location of luminaires for electric lighting simulations.

#### Inputs
* ##### ptsList [Required]
List of points/3d coordinates where the luminaires are to be located.
* ##### spin [Default]
Luminaire spin angle. 
* ##### tilt [Default]
Luminaire tilt angle.
* ##### orientation [Default]
Luminaire rotation angle.
* ##### aimingPoint [Optional]
Location at which the photometric axis of each luminaire should be aimed.
* ##### customLamp [Optional]
Specify a custom lamp using the IES Custom Lamp component

#### Outputs
* ##### readMe!
The execution information, as output and error streams
* ##### luminaireZone
List of coordinates and rotation angles for luminaires


[Check Hydra Example Files for IES Luminaire Zone](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_IES Luminaire Zone)