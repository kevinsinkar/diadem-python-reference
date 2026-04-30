---
title: "IRepD3CharacteristicDiagramPointsAdditionalInt.Marker"
description: "Specifies the markers of the boundary curve points, the maximum and the minimum, and the measuring points in a 3D axis system with the display mode Characterist"
---

# IRepD3CharacteristicDiagramPointsAdditionalInt.Marker

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Marker for 3DAdditionalCharacteristicDiagramPoints

Specifies the markers of the boundary curve points, the maximum and the minimum, and the measuring points in a 3D axis system with the display mode Characteristic diagram in DIAdem REPORT.

## Signature

```python
return_value = obj.Marker
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "\\examples\\data\\engine_characteristic_map.tdm","TDM","")
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
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyMarker = oMyShape.Extensions.BoundaryPoints.Marker
oMyMarker.Type = dd.eMarkerCircle
oMyMarker.Size = 2
oMyMarker.Line.UseCurveColor = False
oMyMarker.Line.Color.SetPredefinedColor(dd.ePredefinedColorDarkGrey)
oMyMarker.Filling.UseCurveColor = False
oMyMarker.Filling.SetPredefinedColor(dd.ePredefinedColorViolet)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Marker_IRepD3CharacteristicDiagramPointsAdditionalInt.htm`*
