---
title: "IRepD2AxisGridLineInt.DotsPerTick"
description: "Specifies the number of gaps between two ticks for the Dots per tick line type in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisGridLineInt.DotsPerTick

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DotsPerTick for 2DAxisGridLine

Specifies the number of gaps between two ticks for the Dots per tick line type in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.DotsPerTick
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
oMy2DAxisSystem.Settings.Grid.DisplayMode = dd.e2DAxisGridModeGrid
oMy2DAxisSystem.Settings.Grid.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
oMyGrid = oMy2DAxisSystem.Settings.Grid
oMyGrid.LineHorizontal.LineType = dd.e2DGridLineTypeDotsPerTick
oMyGrid.LineVertical.LineType = dd.e2DGridLineTypeDotsPerTick
oMyGrid.LineHorizontal.Width = dd.eLineWidth0050
oMyGrid.LineVertical.Width = dd.eLineWidth0050
oMyGrid.LineHorizontal.DotsPerTick = 40
oMyGrid.LineVertical.DotsPerTick = 30
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DotsPerTick_IRepD2AxisGridLineInt.htm`*
