---
title: "IRepD3ShapeObjPointsExtensionsInt.Label"
description: "Specifies the curve labels in the Points display mode in a 3D axis system in DIAdem REPORT."
---

# IRepD3ShapeObjPointsExtensionsInt.Label

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Label for 3DPointsExtensions

Specifies the curve labels in the Points display mode in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Label
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DSurface = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DSurface")
oMySurfaceShape = oMy3DSurface.Shape
oMySurfaceShape.DataStructure = dd.e3DDataStructureMatrix
oMySurfaceShape.XChannel.Reference = "[2]/[1]"
oMySurfaceShape.YChannel.Reference = "[2]/[2]"
oMySurfaceShape.ZChannel.Reference = "[2]/[3]"
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapePoints, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMyShape.Settings.Marker.Type = dd.eMarkerAsterisk
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.ddde"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 6
oMyLabel.Position.Type = dd.e3DLabelPositionAtPoint
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

*Source: `ReportApi/properties/Report_property_Label_IRepD3ShapeObjPointsExtensionsInt.htm`*
