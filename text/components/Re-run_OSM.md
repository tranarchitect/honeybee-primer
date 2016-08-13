## ![](../../images/icons/Re-run_OSM.png) Re-run OSM

![](../../images/components/Re-run_OSM.png)

This is a component for running a previoulsy-generated .osm file through EnergyPlus.

#### Inputs
* ##### osmFilePath [Required]
A file path of the an OpemStdio file
* ##### epwFileAddress [Required]
Address to epw weather file.
* ##### runIt [Required]
Set to "True" to have the component generate an IDF file from the OSM file and run the IDF through through EnergyPlus.  Set to "False" to not run the file (this is the default).  You can also connect an integer for the following options:

#### Outputs
* ##### readMe!
Report!
* ##### idfFileAddress
Script variable Re-Run OSM
* ##### resultFileAddress
The address of the EnergyPlus result file.
* ##### studyFolder
The directory in which the simulation has been run.  Connect this to the 'Honeybee_Lookup EnergyPlus' folder to bring many of the files in this directory into Grasshopper.


[Check Hydra Example Files for Re-run OSM](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Re-run OSM)