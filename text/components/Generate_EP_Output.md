## ![](../../images/icons/Generate_EP_Output.png) Generate EP Output

![](../../images/components/Generate_EP_Output.png)

This component helps select simulation outputs that can be hooked into the WriteIDF component.  Outputs are taken from here:

#### Inputs
* ##### zoneEnergyUse [Optional]
Set to "True" to have EnergyPlus solve for basic building energy use such as heating, cooling, electricity for lights and electricity for plug loads for each zone.
* ##### zoneGainsAndLosses [Optional]
Set to "True" to have EnergyPlus solve for building gains and losses such as people gains, solar gains and infiltration losses/gains.
* ##### zoneComfortMetrics [Optional]
Set to "True" to have EnergyPlus solve for the mean air temperature, mean radiant temperature, operative temperature, and relative humidity of each zone.
* ##### comfortMapVariables [Optional]
Set to "True" to have EnergyPlus solve for the air flow and air heat gain of each zone, which is needed for the comfort map air stratification calculation.
* ##### zoneHVACParams [Optional]
Set to "True" to have EnergyPlus solve for the fractions of heating/cooling loads that are latent vs. sensible as well as the the flow rate and temperature of supply air into each zone.
* ##### surfaceTempAnalysis [Optional]
Set to "True" to have EnergyPlus solve for the interior and exterior surface temperatures of the individual surfaces of each zone.
* ##### surfaceEnergyAnalysis [Optional]
Set to "True" to have EnergyPlus solve for the gains and losses through the individual surfaces of each zone.
* ##### glazingSolarAnalysis [Optional]
Set to "True" to have EnergyPlus solve for the transmitted beam, diffuse, and total solar gain through the individual window surfaces of each zone.  These outputs are needed for Energy Shade Benefit Analysis.
* ##### HBgeneration [Optional]
Set to "True" to have EnergyPlus solve for variables related to HB generation objects like solar panels, wind turbines, batteries, etc.
* ##### timestep [Optional]
Specify a timestep by inputing the words 'hourly', 'daily', 'monthly' or 'annual'.  The default is set to hourly.

#### Outputs
* ##### report
Report!
* ##### simulationOutputs
EnergyPlus code that should be plugged into the "simulationOutputs" parameter of the "writeIDF" component.


[Check Hydra Example Files for Generate EP Output](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Generate EP Output)