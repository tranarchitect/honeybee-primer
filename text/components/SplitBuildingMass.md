## ![](../../images/icons/SplitBuildingMass.png) SplitBuildingMass

![](../../images/components/SplitBuildingMass.png)

Use this component to divide up a brep (polysurface) representative of a complete building massing into smaller volumes that roughly correspond to how a generic EnergyPlus model should be zoned.

#### Inputs
* ##### bldgMasses [Required]
A Closed brep or list of closed breps representing a building massing.
* ##### bldgsFlr2FloorHeights [Optional]
A list of floor heights in Rhino model units that will be used to make each floor of the building.  The list should run from bottom floor to top floor.  Alternatively, you can input a text string that codes for how many floors of each height you want.  For example, inputting "2@4" (without quotations) will make two ground floors with a height of 4 Rhino model units.  Simply typing "@3" will make all floors 3 Rhino model units.  Putting in lists of these text strings will divide up floors accordingly.  For example, the list "1@5   2@4   @3"  will make a ground floor of 5 units, two floors above that at 4 units and all remaining floors at 3 units.
* ##### perimeterZoneDepth [Optional]
A list of perimeter zone depths in Rhino model units that will be used to divide up each floor of the building into core and perimeter zones.  The list should run from bottom floor to top floor.  Alternatively, you can input a text string that codes for which floors you want at which zone depth.  For example, inputting "2@4" (without quotations) will divide up the two ground floors with a perimeter zone depth of 4 Rhino model units.  Simply typing "@3" will divide up all floors with a zone depth of 3 Rhino model units.  Putting in lists of these text strings will divide up floors accordingly.  For example, the list "1@5   2@4   @3"  will make a ground floor divided up with a zone depth of 5 units, two floors divided at 4 units and all remaining floors at 3 units.
* ##### runIt [Required]
Script variable Python

#### Outputs
* ##### readMe!
...
* ##### splitBldgMasses
The building mass split up into zone geometries.


[Check Hydra Example Files for SplitBuildingMass](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_SplitBuildingMass)