---
title: "IRepAxisLabelInt.Font"
description: "Specifies the font of the axis label in an axis system in DIAdem REPORT."
---

# IRepAxisLabelInt.Font

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Font for AxisLabel

Specifies the font of the axis label in an axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Font
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.XAxis.Label.Text = "x-axis"
oMy2DAxisSystem.YAxis.Label.Text = "y-axis"
oMy2DAxisSystem.XAxis.Label.Font.Name = "Times Roman"()
oMy2DAxisSystem.YAxis.Label.Font.Name = "Times Roman"()
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Font_IRepAxisLabelInt.htm`*
