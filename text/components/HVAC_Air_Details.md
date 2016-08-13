## ![](../../images/icons/HVAC_Air_Details.png) HVAC Air Details

![](../../images/components/HVAC_Air_Details.png)

Use this component to set the parameters of a HVAC ventilation system (or air side) that has been assigned with the "Honeybee_Assign HVAC System" component.

#### Inputs
* ##### HVACAvailabiltySched [Default]
A text string representing the HVAC availability that you want to use.  This can be either a shcedule from the schedule libirary or a CSV file path to a CSV schedule you created with the "Honeybee_Create CSV Schedule" component.
* ##### fanTotalEfficiency [Default]
A number between 0 and 1 that represents the overall efficiency of the fan.  Specifically, this is the ratio between the power delivered to the air fluid and the electrical power intput to the fan. It is the product of the motor efficiency and the impeller efficiency.  The impeller efficiency is power delivered to the fluid (air) divided by the shaft power. The power delivered to the fluid is the mass flow rate of the air multiplied by the pressure rise divided by the air density.  The default is usually between 0.6 and 0.7.
* ##### fanMotorEfficiency [Default]
A number between 0 and 1 that represents the efficiency of the fan electric motor.  The motor efficiency is the power delivered to the fan shaft divided by the electrical power input to the motor.  This value must be greater than the _fanTotalEfficiency_ above.  The default is usually around 0.9.
* ##### fanPressureRise [Default]
A number representing the pressure rise across the fan in Pascals.  This is the pressure rise at full flow and standard (sea level) conditions (20°C and 101325 Pa).  The default is usually around 500 Pa.
* ##### fanPlacement [Default]
A boolean value that represents the placement of the fan in relation to cooling or heating coils.  The default is set to True to draw through.  Choose from the following options:
* ##### demandControlledVent [Optional]
A boolean value that represents whether system can vary its speed and the volume of air to match occupancy.  The default is False for all systems.  Choose from the following options:
* ##### heatingSupplyAirTemp [Default]
A number representing the target temperature of the supply air when the system is in heating mode.  For large systems, this is the rated outlet air temperature of the heating coil.  Default for a VAV system is 35C. Default for ideal air is 40 C.
* ##### coolingSupplyAirTemp [Default]
A number representing the target temperature of the supply air when the system is in cooling mode.  For large systems, this is the rated outlet air temperature of the cooling coil.  Default is typically around 12C, which is the coldest temperature before supply air can cause clear thermal discomfort issues. Default for ideal air is 13 C.
* ##### airsideEconomizer [Optional]
An integer or boolean value (0/1) that sets the economizer on the HVAC system.  The default is set to "True" or "1" to include a Differential Dry Bulb air side economizer or "2" for a Differential Enthalpy economizer if the zone has humidity control.  Choose from the following options:
* ##### heatRecovery [Optional]
An integer or boolean value (0/1) that sets the heat recovery on the HVAC system.  The default is set to "False" or 0 to NOT include heat recovery.  Choose from the following options:
* ##### recoveryEffectiveness [Optional]
If the above input has been set to "True", input a number between 0 and 1 here to set the fraction of heat that is recovered by the heat recovery system.  By default, this value is typically around 0.7.

#### Outputs
* ##### airDetails
A description of the HVAC ventilation system (or system air side), which can be plugged into "Honeybee_HVAC Systems" component.


[Check Hydra Example Files for HVAC Air Details](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_HVAC Air Details)