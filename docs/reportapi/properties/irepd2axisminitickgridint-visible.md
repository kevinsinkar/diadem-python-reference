---
title: "IRepD2AxisMiniTickGridInt.Visible"
description: "Specifies whether DIAdem REPORT plots grid lines at the miniticks of the axes in a 2D axis system."
---

# IRepD2AxisMiniTickGridInt.Visible

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Visible for 2DAxisMiniTick

Specifies whether DIAdem REPORT plots grid lines at the miniticks of the axes in a 2D axis system.

## Signature

```python
obj.Visible
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
oMy2DAxisSystem.Settings.Grid.MiniTickGrid.Visible = True
oMy2DAxisSystem.Settings.Grid.MiniTickGrid.Color.SetPredefinedColor(dd.eColorIndexViolet)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Visible_IRepD2AxisMiniTickGridInt.htm`*
