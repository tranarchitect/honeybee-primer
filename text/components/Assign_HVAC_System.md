## ![](../../images/icons/Assign_HVAC_System.png) Assign HVAC System

![](../../images/components/Assign_HVAC_System.png)

Use this component to assign OpenStudio Systems to your HBZones.  By default, all HBZones are assigned an Ideal Air Loads system and this component can be used to change this to a real system from the OpenStudioHVACSystemsList component.

#### Inputs
* ##### HBZones [Required]
The HBZones for which you want to change/adjust the HVAC system.
* ##### HVACSystems [Required]
A HVAC system template from the "Honeybee_HVACSystemsList" component.  ASHRAE recommends using the following baseline systems for different building types and fuel sources:
* ##### airDetails [Default]
Parameters from the "Honeybee_HVAC Air Details" component. Use these to define the features of the ventilation component (or air side) of the HVAC system.
* ##### heatingDetails [Default]
Parameters from the "Honeybee_HVAC Heating Details" component.  Use these to define the features of the heating plant (or hot water side) of the HVAC system.
* ##### coolingDetails [Default]
Parameters from the "Honeybee_HVAC Cooling Details" component.  Use these to define the features of the cooling plant (or chilled water side) of the HVAC system.

#### Outputs
* ##### readMe!
Script variable OSHVACSystems
* ##### HBZones
HBZones that have been modified to have the assigned _HVACSystems.


[Check Hydra Example Files for Assign HVAC System](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Assign HVAC System)