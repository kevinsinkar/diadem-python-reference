---
title: "IRepD3ShapeObjMatrix2DSettingsInt.ShowHiddenLines"
description: "Specifies whether DIAdem REPORT plots hidden lines in a 3D axis system with a 2D matrix display."
---

# IRepD3ShapeObjMatrix2DSettingsInt.ShowHiddenLines

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowHiddenLines for 3DMatrix2DSettings

Specifies whether DIAdem REPORT plots hidden lines in a 3D axis system with a 2D matrix display.

## Signature

```python
obj.ShowHiddenLines
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
oMySettings.ShowHiddenLines = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowHiddenLines_IRepD3ShapeObjMatrix2DSettingsInt.htm`*
