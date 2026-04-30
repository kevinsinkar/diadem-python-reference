---
title: "IRepD2AxisMiniTickGridInt.LineHorizontal"
description: "Specifies the horizontal lines of a minitick grid in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisMiniTickGridInt.LineHorizontal

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineHorizontal for 2DAxisMiniTick

Specifies the horizontal lines of a minitick grid in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.LineHorizontal
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.Y1 = 20
oMyPos.X2 = 80
oMyPos.Y2 = 80
oMy2DAxisSystem.Settings.Grid.DisplayMode = dd.e2DAxisGridModeGrid
oMy2DAxisSystem.Settings.Grid.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
oMyMinitickGrid = oMy2DAxisSystem.Settings.Grid.MiniTickGrid
oMyMinitickGrid.Visible = True
oMyMinitickGrid.LineHorizontal.LineType = dd.eLineTypeDashed1
oMyMinitickGrid.LineHorizontal.Interval = 3
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

*Source: `ReportApi/properties/Report_property_LineHorizontal_IRepD2AxisMiniTickGridInt.htm`*
