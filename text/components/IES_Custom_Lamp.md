## ![](../../images/icons/IES_Custom_Lamp.png) IES Custom Lamp

![](../../images/components/IES_Custom_Lamp.png)

This component can be used to specify a lamp of custom chromaticity, color or color temperature. 

#### Inputs
* ##### lampName [Required]
Specify a name for the lamp.The name can be a predefined lamp name or any other name.
* ##### colorTemp [Default]
Specify a color temperature for the lamp.The color temperature will be used to calculate the chromatcity coordinates of the lamp on the CIE 1931 xy diagram. Lumen depreciation factor for the lamp can be set by specifying a value for the _deprFactor_ input. Valid values for color temperature are from 1000 to 25000.
* ##### xCor [Default]
Specify a chromaticity coordinate for the lamp. The default coordinate is the x coordinate for the CIE 1931 Color Space.
* ##### yCor [Default]
Specify a chromaticity coordinate for the lamp. The default coordinate is the y coordinate for the CIE 1931 Color Space.
* ##### colorSpace [Default]
Specify a color space for the chromaticity coordinates. The values and their corresponding color spaces are
* ##### rgbColors [Default]
Specify a (r,g,b) color value using either the Grasshopper Colour Swatch (preferred) or a text panel. If the alpha value for the Colour Swatch is set to a value other than 255 then that value will be multiplied with the _deprFactor_.
* ##### deprFactor [Default]
Lamp lumen depreciation factor.

#### Outputs
* ##### readMe!
The execution information, as output and error streams
* ##### lampDetails
Information about the lamp defined as per the input parameters.
* ##### customLamp
Connect this to the customLamp_ input in the Honeybee_IES Luminaire option.


[Check Hydra Example Files for IES Custom Lamp](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_IES Custom Lamp)