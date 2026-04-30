---
title: "IRepD2AxisGridInt"
description: "The 2DAxisGrid object provides the grid properties, the axis properties, and the frame properties in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisGridInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAxisGrid

The 2DAxisGrid object provides the grid properties, the axis properties, and the frame properties in a 2D axis system in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2axisgridint-color/">Color</a> | <a href="../../properties/irepd2axisgridint-displaymode/">DisplayMode</a> | <a href="../../properties/irepd2axisgridint-linehorizontal/">LineHorizontal</a> | <a href="../../properties/irepd2axisgridint-linevertical/">LineVertical</a> | <a href="../../properties/irepd2axisgridint-minitickgrid/">MiniTickGrid</a> | <a href="../../properties/irepd2axisgridint-synchronizationmode/">SynchronizationMode</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axissettingsint/">2DAxisSettings</a>.<a href="../../properties/irepd2axissettingsint-grid/">Grid</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisGridInt.htm`*
