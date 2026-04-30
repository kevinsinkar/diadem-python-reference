---
title: "IRepD3ShapeObjCharacteristicDiagramExtensionsInt.MeasurementPoints"
description: "Specifies the properties of the measurement points in a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT."
---

# IRepD3ShapeObjCharacteristicDiagramExtensionsInt.MeasurementPoints

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MeasurementPoints for 3DCharacteristicDiagramExtensions

Specifies the properties of the measurement points in a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.MeasurementPoints
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
oMyShape.Extensions.MeasurementPoints.Visible = True
oMyLabel = oMyShape.Extensions.MeasurementPoints.Label
oMyLabel.Visible = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MeasurementPoints_IRepD3ShapeObjCharacteristicDiagramExtensionsInt.htm`*
