## ![](../../images/icons/Apply_OpenStudio_Measure.png) Apply OpenStudio Measure

![](../../images/components/Apply_OpenStudio_Measure.png)

This component applies an OpenStudio measure to an OpenStudio file. The component will eventually be integrated to Export to OpenStudio component.

#### Inputs
* ##### osmFilePath [Required]
A file path of the an OpemStdio file
* ##### epwWeatherFile [Required]
An .epw file path on your system as a text string.
* ##### OSMeasure [Required]
Loaded OpenStudio measure. Use load OpenStudio measures to load the measure to Honeybee
* ##### runIt [Required]
set to True to apply the measure and run the analysis

#### Outputs
* ##### ReadMe!
The execution information, as output and error streams
* ##### projectFolder
Path to new project folder
* ##### modifiedIdfFilePath
Path to modified EnergyPlus file
* ##### modifiedOsmFilePath
Path to modified OpenStudio file
* ##### resultsFileAddress
Path to .csv results file


[Check Hydra Example Files for Apply OpenStudio Measure](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Apply OpenStudio Measure)