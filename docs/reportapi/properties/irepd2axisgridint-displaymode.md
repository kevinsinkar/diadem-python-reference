---
title: "IRepD2AxisGridInt.DisplayMode"
description: "Specifies whether DIAdem REPORT only displays axes, or whether DIAdem REPORT also displays frames and grid lines in a 2D axis system."
---

# IRepD2AxisGridInt.DisplayMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DisplayMode for 2DAxisGrid

Specifies whether DIAdem REPORT only displays axes, or whether DIAdem REPORT also displays frames and grid lines in a 2D axis system.

## Signature

```python
obj.DisplayMode
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DisplayMode_IRepD2AxisGridInt.htm`*
