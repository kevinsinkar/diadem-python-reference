---
title: "IRepD3CharacteristicDiagramHyperbolaAdditionalInt.InsideBoundary"
description: "Specifies whether DIAdem displays hyperbolas in a characteristic diagram only within the boundary curve . DIAdem only includes this property if hyperbolas are v"
---

# IRepD3CharacteristicDiagramHyperbolaAdditionalInt.InsideBoundary

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: InsideBoundary for 3DAdditionalHyperbolaLines

Specifies whether DIAdem displays hyperbolas in a characteristic diagram only within the boundary curve . DIAdem only includes this property if hyperbolas are visible and you assign the value True to the Visible for 3DAdditionalHyperbolaLines property.

## Signature

```python
obj.InsideBoundary
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\" + "engine_characteristic_map","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.ZChannel.Reference = "[1]/[3]"
oMySettings = oMy3DAxisSystem.Settings
oMySettings.RotationAngleXY = 90
oMySettings.RotationAngleZ = 270
oMyShape.Extensions.BoundaryCurve.Visible = True
oMyShape.Extensions.Hyperbola.Visible = True
oMyShape.Extensions.Hyperbola.InsideBoundary = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_InsideBoundary_IRepD3CharacteristicDiagramHyperbolaAdditionalInt.htm`*
