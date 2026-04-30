---
title: "IRepD2ShapeObjBarsHorizontalSettingsInt.Offset"
description: "Specifies the displacement of the bars as a percentage when DIAdem displays horizontal bars in a 2D axis system in DIAdem REPORT. The entry is a percentage of t"
---

# IRepD2ShapeObjBarsHorizontalSettingsInt.Offset

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Offset for 2DBarsHorizontalSettings

Specifies the displacement of the bars as a percentage when DIAdem displays horizontal bars in a 2D axis system in DIAdem REPORT. The entry is a percentage of the maximum bar width.

## Signature

```python
obj.Offset
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBarsHorizontal, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "[4]/[1]"
oMySettings = oMyShape.Settings
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Filling.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
oMySettings.Width = 25
oMySettings.Offset = 50
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Offset_IRepD2ShapeObjBarsHorizontalSettingsInt.htm`*
