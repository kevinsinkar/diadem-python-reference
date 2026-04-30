---
title: "IRepD3ShapeObjBarsSettingsInt.Dimensions"
description: "Specifies the width and the displacement of the bars in a 3D axis system in the Bars display mode in DIAdem REPORT."
---

# IRepD3ShapeObjBarsSettingsInt.Dimensions

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Dimensions for 3DBarsSettings

Specifies the width and the displacement of the bars in a 3D axis system in the Bars display mode in DIAdem REPORT.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeBars, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyDimensions = oMyShape.Settings.Dimensions
oMyDimensions.OffsetX = 10
oMyDimensions.OffsetY = 10
oMyDimensions.WidthX = 5
oMyDimensions.WidthY = 5
oMyLineSettings = oMyShape.Settings.Line
oMyLineSettings.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyLineSettings.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Dimensions_IRepD3ShapeObjBarsSettingsInt.htm`*
