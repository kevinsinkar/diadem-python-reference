---
title: "IRepD2AxisGridLineInt.Interval"
description: "Specifies the number of gaps between two ticks for broken grid lines in a 2D axis system in DIAdem REPORT. For the Dots per tick line style, use the DotsPerTick"
---

# IRepD2AxisGridLineInt.Interval

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Interval for 2DAxisGridLine

Specifies the number of gaps between two ticks for broken grid lines in a 2D axis system in DIAdem REPORT. For the Dots per tick line style, use the DotsPerTick property to specify the number of gaps between two ticks.

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
oMyPos.Y1 = 20
oMyPos.X2 = 80
oMyPos.Y2 = 80
oMy2DAxisSystem.Settings.Grid.DisplayMode = dd.e2DAxisGridModeGrid
oMy2DAxisSystem.Settings.Grid.LineHorizontal.LineType = dd.e2DGridLineTypeDashDot
oMy2DAxisSystem.Settings.Grid.LineHorizontal.Interval = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Interval_IRepD2AxisGridLineInt.htm`*
