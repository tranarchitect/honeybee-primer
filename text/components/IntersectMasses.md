## ![](../../images/icons/IntersectMasses.png) IntersectMasses

![](../../images/components/IntersectMasses.png)

Use this component to take a list of closed breps (polysurfaces) that you intend to turn into HBZones and split their component surfaces to ensure that there are matching surfaces between each of the adjacent zones.

#### Inputs
* ##### bldgMassesBefore [Required]
Script input bldgMassesBefore.

#### Outputs
* ##### bldgMassesAfter
The same input closed breps that have had their component surfaces split by adjacent polysurfaces to have matching surfaces between adjacent breps.  It is recommended that you bake this output and check it in Rhino before turning the breps into HBZones.


[Check Hydra Example Files for IntersectMasses](https://hydrashare.github.io/hydra/index.html?keywords=Honeybee_IntersectMasses)