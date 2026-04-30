---
title: "IRepD2AxisYInt.Label"
description: "Specifies the label of the y-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYInt.Label

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Label for 2DAxisY

Specifies the label of the y-axis in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Label
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
oMyYLabel = oMy2DAxisSystem.YAxis.Label
oMyYLabel.Text = "This is the y-axis"
oMyYLabel.Angle = 90
oMyYLabel.Font.Name = "Tahoma"
oMyYLabel.Font.Size = 7
oMyYLabel.OffsetX = 100
oMyYLabel.OffsetY = -10
oMyYLabel.RelativePosition = dd.eAxisLabelRelativePositionRight
oMyXLabel = oMy2DAxisSystem.XAxis.Label
oMyXLabel.UseCurveColor = True
oMyXLabel.Text = "This is the x-axis"
oMyXLabel.Angle = 0
oMyXLabel.Font.Name = "Tahoma"
oMyXLabel.Font.Size = 7
oMyXLabel.OffsetX = -7
oMyXLabel.OffsetX = 100
oMyXLabel.RelativePosition = dd.eAxisLabelRelativePositionRight
oMyXLabel.UseCurveColor = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Label_IRepD2AxisYInt.htm`*
