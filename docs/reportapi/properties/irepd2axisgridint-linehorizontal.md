---
title: "IRepD2AxisGridInt.LineHorizontal"
description: "Specifies the horizontal grid lines in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisGridInt.LineHorizontal

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineHorizontal for 2DAxisGrid

Specifies the horizontal grid lines in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.LineHorizontal
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
oMyGrid = oMy2DAxisSystem.Settings.Grid
oMyGrid.DisplayMode = dd.e2DAxisGridModeGrid
oMyGrid.LineHorizontal.LineType = dd.e2DGridLineTypeDashed1
oMyGrid.LineHorizontal.Interval = 3
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_LineHorizontal_IRepD2AxisGridInt.htm`*
