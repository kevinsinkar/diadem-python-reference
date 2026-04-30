---
title: "IRepD2AxisMiniTickGridInt.Color"
description: "Specifies the color of the minitick grid in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisMiniTickGridInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for 2DAxisMiniTick

Specifies the color of the minitick grid in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Color
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
oMy2DAxisSystem.Settings.Grid.MiniTickGrid.Visible = True
oMy2DAxisSystem.Settings.Grid.MiniTickGrid.Color.SetPredefinedColor(dd.eColorIndexViolet)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepD2AxisMiniTickGridInt.htm`*
