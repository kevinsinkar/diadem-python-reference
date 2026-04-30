---
title: "IRepD2AxisGridInt.SynchronizationMode"
description: "Specifies whether DIAdem REPORT aligns the ticks of the subaxes to the main axes in a 2D axis system."
---

# IRepD2AxisGridInt.SynchronizationMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SynchronizationMode for 2DAxisGrid

Specifies whether DIAdem REPORT aligns the ticks of the subaxes to the main axes in a 2D axis system.

## Signature

```python
obj.SynchronizationMode
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
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.Settings.Grid.DisplayMode =dd.e2DAxisGridModeGrid
oMy2DAxisSystem.YAxisList.Add("MySecondYAxis")
oMy2DAxisSystem.Settings.Grid.SynchronizationMode = dd.e2DGridSynchronizationGrid
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SynchronizationMode_IRepD2AxisGridInt.htm`*
