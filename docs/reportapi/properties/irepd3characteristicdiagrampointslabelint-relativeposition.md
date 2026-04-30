---
title: "IRepD3CharacteristicDiagramPointsLabelInt.RelativePosition"
description: "Specifies the relative position of the symbol labels to the curve data points which DIAdem REPORT uses in the Characteristic diagram display mode."
---

# IRepD3CharacteristicDiagramPointsLabelInt.RelativePosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativePosition for 3DCharacteristicDiagramPointsLabel

Specifies the relative position of the symbol labels to the curve data points which DIAdem REPORT uses in the Characteristic diagram display mode.

## Signature

```python
obj.RelativePosition
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eRelativePositionRightTop` | 0 | Top right |
| `eRelativePositionCenter` | 1 | Center |
| `eRelativePositionRight` | 2 | Right |
| `eRelativePositionRightBottom` | 3 | Bottom right |
| `eRelativePositionTop` | 4 | Top |
| `eRelativePositionBottom` | 5 | Bottom |
| `eRelativePositionLeftTop` | 6 | Top left |
| `eRelativePositionLeft` | 7 | Left |
| `eRelativePositionLeftBottom` | 8 | Bottom left |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "\\examples\\data\\engine_characteristic_map.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMySettings = oMy3DAxisSystem.Settings
oMySettings.RotationAngleXY = 90
oMySettings.RotationAngleZ = 270
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.ZChannel.Reference = "[1]/[3]"
oMyShape.Extensions.BoundaryCurve.Visible = True
oMyShape.Extensions.BoundaryPoints.Visible = True
oMyLabel = oMyShape.Extensions.BoundaryPoints.Label
oMyLabel.Visible = True
oMyLabel.Font.Size = 4
oMyLabel.RelativePosition = dd.eRelativePositionCenter
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RelativePosition_IRepD3CharacteristicDiagramPointsLabelInt.htm`*
