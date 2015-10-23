## ![](../../images/icons/Add_Internal_Mass_to_Zone.png) Add Internal Mass to Zone

![](../../images/components/Add_Internal_Mass_to_Zone.png)

Use this component to assign internal thermal masses to zones, which can be used to account for the effects of furniture inside zones or massive building components like hearths and chimneys.

#### Inputs
* ##### HBZones [Required]
HBZones for which internal masses are to be assigned.
* ##### internalMassName [Optional]
An optional text name for the internal mass.  This can be useful for keeping track of different internal mass types if you use several of this component in series.
* ##### srfsOrSrfArea [Required]
A list of Rhino breps representing the surfaces of internal masses (or furniture) that are exposed to the air of the zone.  Alternatively, this can be a number or list of numbers representing the surface area of the internal masses (or furniture) that are exposed to the zone air.
* ##### EPConstruction [Required]
An EnergyPlus Construction that represents the type of material that the thermal mass is composed of.  This can be either a construction from the "Call from EP Construction Library" component or a custom construction from the "EnergyPlus Construction" component.

#### Outputs
* ##### readMe!
The execution information, as output and error streams
* ##### HBZones
HBZones with internal masses assigned.


[Check Hydra Example Files for Add Internal Mass to Zone](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Add Internal Mass to Zone)