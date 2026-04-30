---
title: "IRepAxisLabelInt.RelativePosition"
description: "Specifies the relative position of the axis label to the axis in an axis system in DIAdem REPORT."
---

# IRepAxisLabelInt.RelativePosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativePosition for AxisLabel

Specifies the relative position of the axis label to the axis in an axis system in DIAdem REPORT.

## Signature

```python
obj.RelativePosition
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAxisLabelRelativePositionManual` | 0 | Manual |
| `eAxisLabelRelativePositionCentric` | 1 | Centered |
| `eAxisLabelRelativePositionRight` | 2 | Right |
| `eAxisLabelRelativePositionLeft` | 3 | Left |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.XAxis.Label.Text = "This is the x-axis"
oMy2DAxisSystem.YAxis.Label.Text = "This is the y-axis"
oMy2DAxisSystem.XAxis.Label.RelativePosition = dd.eAxisLabelRelativePositionCentric
oMy2DAxisSystem.YAxis.Label.RelativePosition = dd.eAxisLabelRelativePositionCentric
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RelativePosition_IRepAxisLabelInt.htm`*
