## ![](../../images/icons/Generate_Cumulative_Sky.png) Generate Cumulative Sky

![](../../images/components/Generate_Cumulative_Sky.png)

This component generate a cumulative sky using GenCumulativeSky.exe. Only and only use it for radiation analysis (no daylighting!)

#### Inputs
* ##### weatherFile [Required]
epw weather file address on your system
* ##### analysisPeriod [Default]
Indicates the analysis period. An annual study will be run if this input is not provided by the user
* ##### generateSky [Required]
Set boolean to True to run the component

#### Outputs
* ##### skyFilePath
Sky file location on the local drive


[Check Hydra Example Files for Generate Cumulative Sky](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_Generate Cumulative Sky)