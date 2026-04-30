---
title: "IRepD3ShapeObjBarsSettingsInt.ShowHiddenLines"
description: "Specifies whether DIAdem REPORT plots hidden lines in a 3D axis system with a bar display."
---

# IRepD3ShapeObjBarsSettingsInt.ShowHiddenLines

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowHiddenLines for 3DBarsSettings

Specifies whether DIAdem REPORT plots hidden lines in a 3D axis system with a bar display.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeBars, "MyNew3DCurve")
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

*Source: `ReportApi/properties/Report_property_ShowHiddenLines_IRepD3ShapeObjBarsSettingsInt.htm`*
