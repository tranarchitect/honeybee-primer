## ![](../../images/icons/Re-run_IDF.png) Re-run IDF

![](../../images/components/Re-run_IDF.png)

This is a component for running a previoulsy-generated .idf file through EnergyPlus with a different weather file.

#### Inputs
* ##### workingDir []
The working directory of the energyPlus idf.
* ##### idfFileName []
Name of the idf file (e.g. sample1.idf).
* ##### epwFileAddress []
Address to epw weather file.
* ##### EPDirectory []
[Optional] where EnergyPlus is installed on your system
* ##### runIt []
Set to 'True' to run the simulation.

#### Outputs
* ##### report
Report!
* ##### resultFileAddress
The address of the EnergyPlus result file.


[Check Hydra Example Files for Re-run IDF](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Re-run IDF)