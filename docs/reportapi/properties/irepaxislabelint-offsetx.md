---
title: "IRepAxisLabelInt.OffsetX"
description: "Specifies the margin of the axis label in the x-direction as a percentage of the width of the worksheet in DIAdem REPORT. First assign the value eAxisLabelRelat"
---

# IRepAxisLabelInt.OffsetX

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OffsetX for AxisLabel

Specifies the margin of the axis label in the x-direction as a percentage of the width of the worksheet in DIAdem REPORT. First assign the value eAxisLabelRelativePositionManual to the property RelativePosition .

## Signature

```python
obj.OffsetX
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.XAxis.Label.Text = "x-axis"
oMy2DAxisSystem.YAxis.Label.Text = "y-axis"
oMy2DAxisSystem.XAxis.Label.RelativePosition = dd.eAxisLabelRelativePositionManual
oMy2DAxisSystem.YAxis.Label.RelativePosition = dd.eAxisLabelRelativePositionManual
oMy2DAxisSystem.XAxis.Label.OffsetY = 5
oMy2DAxisSystem.YAxis.Label.OffsetX = 5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OffsetX_IRepAxisLabelInt.htm`*
