## ![](../../images/icons/Read_EP_HVAC_Result.png) Read EP HVAC Result

![](../../images/components/Read_EP_HVAC_Result.png)

This component reads the results of an EnergyPlus simulation from the WriteIDF Component or any EnergyPlus result .csv file address.  Note that, if you use this component without the WriteIDF component, you should make sure that a corresponding .eio file is next to your .csv file at the input address that you specify.

#### Inputs
* ##### resultFileAddress [Required]
The result file address that comes out of the WriteIDF component.
* ##### normByFloorArea [Optional]
Set to 'True' to normalize all zone energy data by floor area (note that the resulting units will be kWh/m2 as EnergyPlus runs in the metric system). The default is set to "False."

#### Outputs
* ##### sensibleCooling
The sensible energy removed by the ideal air cooling load for each zone in kWh.
* ##### latentCooling
The latent energy removed by the ideal air cooling load for each zone in kWh.
* ##### sensibleHeating
The sensible energy added by the ideal air heating load for each zone in kWh.
* ##### latentHeating
The latent energy added by the ideal air heating load for each zone in kWh.
* ##### supplyMassFlow
The mass of supply air flowing into each zone in kg/s.
* ##### supplyAirTemp
The mean air temperature of the supply air for each zone (degrees Celcius).
* ##### supplyAirHumidity
The relative humidity of the supply air for each zone (%).
* ##### earthTubeCooling
The sensible energy removed by an earth tube system for each zone in kWh.
* ##### earthTubeHeating
The sensible energy added by an earth tube system for each zone in kWh.


[Check Hydra Example Files for Read EP HVAC Result](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Read EP HVAC Result)