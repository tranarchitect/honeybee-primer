## ![](../../images/icons/EnergyPlus_Construction.png) EnergyPlus Construction

![](../../images/components/EnergyPlus_Construction.png)

Use this component to make your own EnergyPlus construction.  Inputs can be either the name of a matterial form the Openstudio construction library or a custom material made with any of the EnergyPlus Material components.

#### Inputs
* ##### name [Required]
A text name for your custom construction. This is what you will use as an input to other components in order to reference your custom construction.
* ##### layer_1 [Required]
The first and outer-most layer of your construction.
* ##### layer_2 [Required]
The second outer-most layer of your construction.
* ##### layer_3 [Required]
The third outer-most layer of your construction.

#### Outputs
* ##### EPConstruction
An EnergyPlus construction that can be plugged into the "Honeybee_Add to EnergyPlus Library" component in order to write the construction into the project library.


[Check Hydra Example Files for EnergyPlus Construction](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_EnergyPlus Construction)