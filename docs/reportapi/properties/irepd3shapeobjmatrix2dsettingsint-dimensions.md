---
title: "IRepD3ShapeObjMatrix2DSettingsInt.Dimensions"
description: "Specifies the width and the displacement of the matrix in a 3D axis system in the 2D matrix display mode in DIAdem REPORT."
---

# IRepD3ShapeObjMatrix2DSettingsInt.Dimensions

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Dimensions for 3DMatrix2DSettings

Specifies the width and the displacement of the matrix in a 3D axis system in the 2D matrix display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.Dimensions
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeMatrix2D, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Dimensions.WidthX = 10
oMySettings.Dimensions.WidthY = 10
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue )
oMySettings.Line.Width = dd.eLineWidth0025
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.ddde"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 8
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

*Source: `ReportApi/properties/Report_property_Dimensions_IRepD3ShapeObjMatrix2DSettingsInt.htm`*
