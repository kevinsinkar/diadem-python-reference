---
title: "IRepAxisMiniTickGridLineInt.Interval"
description: "Specifies the interval and the length of the line sections of the broken minitick lines in a 2D axis system in DIAdem REPORT. Greater values mean greater interv"
---

# IRepAxisMiniTickGridLineInt.Interval

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Interval for AxisMiniTickGridLine

Specifies the interval and the length of the line sections of the broken minitick lines in a 2D axis system in DIAdem REPORT. Greater values mean greater intervals.

## Signature

```python
obj.Interval
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMySettings = oMy2DAxisSystem.Settings
oMySettings.Grid.DisplayMode = dd.e2DAxisGridModeGrid
oMySettings.Grid.MiniTickGrid.Visible = True
oMyHMiniTick = oMySettings.Grid.MiniTickGrid.LineHorizontal
oMyHMiniTick.Interval = 10
oMyHMiniTick.LineType = dd.eLineTypeDashDot
oMyHMiniTick.Width = dd.eLineWidth0100
oMyVMiniTick = oMySettings.Grid.MiniTickGrid.LineVertical
oMyVMiniTick.Interval = 10
oMyVMiniTick.LineType = dd.eLineTypeDashDot
oMyVMiniTick.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Interval_IRepAxisMiniTickGridLineInt.htm`*
