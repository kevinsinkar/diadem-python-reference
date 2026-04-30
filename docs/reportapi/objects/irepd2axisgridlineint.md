---
title: "IRepD2AxisGridLineInt"
description: "The 2DAxisGrid object provides the grid properties of a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisGridLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAxisGridLine

The 2DAxisGrid object provides the grid properties of a 2D axis system in DIAdem REPORT.

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
#oMySettings.Grid.MiniTickGrid.Visible = True
oMyHLine = oMySettings.Grid.LineHorizontal
oMyHLine.LineType = dd.e2DGridLineTypeDashDot
oMyHLine.Interval = 5
oMyHLine.Width = dd.eLineWidth0100
oMyVLine = oMySettings.Grid.LineVertical
oMyVLine.LineType = dd.e2DGridLineTypeDotsPerTick
oMyVLine.DotsPerTick = 10
oMyVLine.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2axisgridlineint-dotspertick/">DotsPerTick</a> | <a href="../../properties/irepd2axisgridlineint-interval/">Interval</a> | <a href="../../properties/irepd2axisgridlineint-linetype/">LineType</a> | <a href="../../properties/irepd2axisgridlineint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisgridint/">2DAxisGrid</a>.<a href="../../properties/irepd2axisgridint-linehorizontal/">LineHorizontal</a> | <a href="../irepd2axisgridint/">2DAxisGrid</a>.<a href="../../properties/irepd2axisgridint-linevertical/">LineVertical</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisGridLineInt.htm`*
