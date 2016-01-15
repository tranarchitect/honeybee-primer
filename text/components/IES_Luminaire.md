## ![](../../images/icons/IES_Luminaire.png) IES Luminaire

![](../../images/components/IES_Luminaire.png)

This is the core component for adding photometric data into a lighting simulation. 

#### Inputs
* ##### iesFilePath [Required]
Specify the file path for .ies photometry file.
* ##### luminaireID [Required]
Custom name for the luminaire rad file. The default name is the same as the name of the IES file.
* ##### luminaireZone [Required]
List of (3-d coordinate, Aiming Angle) combinations that are generated through the IES Luminaire Array component.
* ##### lightLossFactor [Default]
Optional value for light loss factor. Default is 1.0
* ##### candelaMultiplier [Default]
Assign a scaling value for the candela tables. This value gets multiplied by the _lightLossFactor_ value.
* ##### customLamp [Optional]
Specify a custom lamp using the IES Custom Lamp component
* ##### drawLuminaireWeb [Default]
Draw a geometric representation of the candela distribution of the luminaire on the Rhino viewport. If set to True then geometry normalized to unit dimensions will be drawn. If a number is provided, then geometry will be drawn and scaled to that value.
* ##### drawLuminaireAxes [Default]
Draw the C0-G0 axes of the luminaire on the Rhino viewport. If set to True then axes normalized to 1.5 times the unit dimensions will be drawn. If a number is provided, then geometry will be drawn and scaled to that value.
* ##### drawLuminairePoly [Default]
Draw the polygon, circle or box representing the luminous opening of the luminaire on the Rhino viewport. If set to True then geometry normalized to unit dimensions will be drawn. If a number is provided, then geometry will be drawn and scaled to that value.
* ##### extendLumAxesToPt [Optional]
Specify a point to which the luminaire axes should be extended to. Please note that if the aiming of the luminaire is very far way from this point then some abnormal results might be seen.
* ##### radDir [Default]
Custom location for the luminaire rad file. The default location is the same as where the original IES file is located.
* ##### writeRad [Required]
Set to True to create the file for electric lighting simulation.

#### Outputs
* ##### readMe!
The execution information, as output and error streams
* ##### luminaireDetails
A description of the luminaire generated after parsing the IES file.
* ##### luminaire3dWeb
The geometry created in the Rhino viewport for visualizing the luminaire. Can be used for generating previews.
* ##### luminaireList
List of luminaires and their locations and mounting angles.
* ##### radFilePath
Location of the RAD file that should be included in the project. Connect this output to the _additionalRadFiles_ input in the Honeybee_Run_DaylightSimulation module.


[Check Hydra Example Files for IES Luminaire](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_IES Luminaire)