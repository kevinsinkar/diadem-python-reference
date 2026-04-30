---
title: "IRepD3ShapeObjLineSettingsInt.Line"
description: "Specifies the properties of the curve line in the 3D curve display mode in a 3D axis system in DIAdem REPORT."
---

# IRepD3ShapeObjLineSettingsInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for 3DLineSettings

Specifies the properties of the curve line in the 3D curve display mode in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeLine, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[3]/[1]"
oMyShape.YChannel.Reference = "[3]/[2]"
oMyShape.ZChannel.Reference = "[3]/[3]"
oMyShape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyShape.Settings.Line.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepD3ShapeObjLineSettingsInt.htm`*
