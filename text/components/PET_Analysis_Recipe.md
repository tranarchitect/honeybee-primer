## ![](../../images/icons/PET_Analysis_Recipe.png) PET Analysis Recipe

![](../../images/components/PET_Analysis_Recipe.png)

Use this component to assemble an adaptive comfort recipe for the "Honeybee_Annual Indoor Comfort Analysis" component.

#### Inputs
* ##### viewFactorMesh [Required]
The data tree of view factor meshes that comes out of the  "Honeybee_Indoor View Factor Calculator".
* ##### viewFactorInfo [Required]
The python list that comes out of the  "Honeybee_Indoor View Factor Calculator".
* ##### epwFile [Required]
The epw file that was used to run the EnergyPlus model.  This will be used to generate sun vectors and get radiation data for estimating the temperature delta for sun falling on occupants.
* ##### srfIndoorTemp [Optional]
A list surfaceIndoorTemp data out of the "Honeybee_Read EP Surface Result" component.
* ##### srfOutdoorTemp [Required]
A list surfaceOutdoorTemp data out of the "Honeybee_Read EP Surface Result" component.
* ##### zoneAirTemp [Optional]
The airTemperature output of the "Honeybee_Read EP Result" component.
* ##### zoneRelHumid [Optional]
The relativeHumidity output of the "Honeybee_Read EP Result" component.
* ##### zoneAirFlowVol [Optional]
The airFlowVolume output of the "Honeybee_Read EP Result" component.
* ##### zoneAirHeatGain [Optional]
The airHeatGainRate output of the "Honeybee_Read EP Result" component.
* ##### bodyCharacteristics [Optional]
A list of body characteristics in the following order: age, sex, height, weight, bodyPosition, clothingInsulation, acclimated, metabolicRate, activityDuration.
* ##### temperateOrTropical [Optional]
Set to "True" to have the component use the tropical/subtropical/humid categories to determine whether the conditions are cold, hot, or comfortable.  Set to "False" to use categories for a temperate climate.  The tropical categories were determined by Lin and Matzarakis (2008) and the temperate categories were determined by Matzarakis and Mayer (1996). The default is set to "True" for tropical/subtropical categories.
* ##### wellMixedAirOverride [Optional]
Set to "True" if you know that your building will have a forced air system with diffusers meant to mix the air as well as possilbe.  This will prevent the calculation from running the air stratification function and instead assume well mixed conditions.  This input can also be a list of 8760 boolean values that represent the hours of the year when a forced air system or ceiling fans are run to mix the air.  The default is set to 'False' to run the stratification calculation for every hour of the year, assuming no forced air heating/cooling system.
* ##### inletHeightOverride [Optional]
An optional list of float values that match the data tree of view factor meshes and represent the height, in meters, from the bottom of the view factor mesh to the window inlet height.  This will override the default value used in the air stratification calculation, which sets the inlet height in the bottom half of the average glazing height.
* ##### windowShadeTransmiss [Optional]
A decimal value between 0 and 1 that represents the transmissivity of the shades on the windows of a zone (1 is no shade and 0 is fully shaded).  This input can also be a list of 8760 values between 0 and 1 that represents a list of hourly window shade transmissivities to be applied to all windows of the model. Finally and most importantly, this can be the 'windowTransmissivity' output of the 'Read EP Surface Result' component for an energy model that has been run with window shades.  This final option ensures that the energy model and the confort map results are always aligned although it is the most computationally expensive of the options.  The default is set to 0, which assumes no additional shading to windows. 
* ##### cloAbsorptivity [Optional]
An optional decimal value between 0 and 1 that represents the fraction of solar radiation reflected off of the ground.  By default, this is set to 0.25, which is characteristic of most indoor floors.  You may want to increase this value for concrete or decrease it for dark carpets.
* ##### windSpeed [Optional]
A value in m/s to set the wind speed of the comfort calculation. Use this input to account for objects like ceiling fans that might increase the interior wind speed or input custom wind speed values from a CFD simulation.
* ##### outdoorTerrain [Optional]
An interger or text string that sets the terrain class associated with the wind speed used in outdoor wind calculations. Interger values represent the following terrain classes:
* ##### north [Optional]
Input a vector to be used as a true North direction for the comfort analysis or a number between 0 and 360 that represents the degrees off from the y-axis to make North.  The default North direction is set to the Y-axis (0 degrees).

#### Outputs
* ##### comfRecipe
An analysis recipe for the "Honeybee_Annual Indoor Comfort Analysis" component.


[Check Hydra Example Files for PET Analysis Recipe](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_PET Analysis Recipe)