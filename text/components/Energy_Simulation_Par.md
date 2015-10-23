## ![](../../images/icons/Energy_Simulation_Par.png) Energy Simulation Par

![](../../images/components/Energy_Simulation_Par.png)

EnergyPlus Shadow Parameters

#### Inputs
* ##### timestep [Optional]
A number between 1 and 60 that represents the number of timesteps per hour at which the simulation will be run.  The default is set to 6 timesteps per hour, which means that the energy balance calculation is run every 10 minutes of the year.
* ##### shadowCalcPar [Optional]
An optional set of shadow calculation parameters from the "Honeybee_ShadowPar" component.
* ##### solarDistribution [Optional]
An optional text string or integer that sets the solar distribution calculation.  Choose from the following options:
* ##### simulationControls [Optional]
An optional set of simulation controls from the "Honeybee_Simulation Control" component.
* ##### ddyFile [Optional]
An optional file path to a .ddy file on your system.  This ddy file will be used to size the HVAC system before running the simulation.
* ##### terrain [Optional]
An optional integer or text string to set the surrouning terrain of the building, which will be used to determine how wind speed around the building changes with height.  If no value is input here, the default is set to "City."  Choose from the following options:
* ##### monthlyGrndTemps [Optional]
An optional list of 12 monthly ground temperatures to be used by those surfaces in contact with the ground in the simulation.  Please note that the EPW values out of the Import Ground Temp component are usually too extreme for a conditioned building.  If no values are input here, the model will attempt to estimate a reasonable starting base temperature from these results by using a value of 18C in cases of monthly ground temperatures below 18C, 24C in cases of monthly ground temperatures above 24C, and the actual ground temperature if the monthly average falls in between 18C and 24C.  Usually, ground temperatures will be about 2C lower than the overage indoor air temperature for a given month.

#### Outputs
* ##### energySimPar
Energy simulation parameters that can be plugged into the "Honeybee_ Run Energy Simulation" component.


[Check Hydra Example Files for Energy Simulation Par](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Energy Simulation Par)