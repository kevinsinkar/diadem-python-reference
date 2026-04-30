---
title: "IRepD3ShapeObj2DMatrixInt.Settings"
description: "Specifies the properties of a 2D-Matrix in the Bars display mode in DIAdem REPORT."
---

# IRepD3ShapeObj2DMatrixInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for 3DMatrix2D

Specifies the properties of a 2D-Matrix in the Bars display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.Settings
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Settings_IRepD3ShapeObj2DMatrixInt.htm`*
