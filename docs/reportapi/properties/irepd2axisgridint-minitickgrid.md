---
title: "IRepD2AxisGridInt.MiniTickGrid"
description: "Specifies the minitick grid properties in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisGridInt.MiniTickGrid

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MiniTickGrid for 2DAxisGrid

Specifies the minitick grid properties in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.MiniTickGrid
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
OMyMinitickGrid = oMy2DAxisSystem.Settings.Grid.MiniTickGrid
OMyMinitickGrid.Visible = True
OMyMinitickGrid.LineHorizontal.LineType = dd.eLineTypeDashed1
OMyMinitickGrid.LineHorizontal.Interval = 3
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MiniTickGrid_IRepD2AxisGridInt.htm`*
