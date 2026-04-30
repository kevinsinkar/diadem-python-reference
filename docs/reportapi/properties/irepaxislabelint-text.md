---
title: "IRepAxisLabelInt.Text"
description: "Specifies the axis label in an axis system in DIAdem REPORT."
---

# IRepAxisLabelInt.Text

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Text for AxisLabel

Specifies the axis label in an axis system in DIAdem REPORT.

## Signature

```python
obj.Text
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexGreen)
oMy2DAxisSystem.XAxis.Label.Text = "x-axis"
oMy2DAxisSystem.YAxis.Label.Text = "y-axis"
oMy2DAxisSystem.XAxis.Label.UseCurveColor = True
oMy2DAxisSystem.YAxis.Label.UseCurveColor = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Text_IRepAxisLabelInt.htm`*
