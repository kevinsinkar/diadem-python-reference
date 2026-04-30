---
title: "IRepAxisLabelInt"
description: "The AxisLabel object provides the label of an axis in DIAdem REPORT."
---

# IRepAxisLabelInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: AxisLabel

The AxisLabel object provides the label of an axis in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepaxislabelint-angle/">Angle</a> | <a href="../../properties/irepaxislabelint-font/">Font</a> | <a href="../../properties/irepaxislabelint-offsetx/">OffsetX</a> | <a href="../../properties/irepaxislabelint-offsety/">OffsetY</a> | <a href="../../properties/irepaxislabelint-relativeposition/">RelativePosition</a> | <a href="../../properties/irepaxislabelint-text/">Text</a> | <a href="../../properties/irepaxislabelint-usecurvecolor/">UseCurveColor</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisxint/">2DAxisX</a>.<a href="../../properties/irepd2axisxint-label/">Label</a> | <a href="../irepd2axisyint/">2DAxisY</a>.<a href="../../properties/irepd2axisyint-label/">Label</a> | <a href="../irepd3axisxint/">3DAxisX</a>.<a href="../../properties/irepd3axisxint-label/">Label</a> | <a href="../irepd3axisyint/">3DAxisY</a>.<a href="../../properties/irepd3axisyint-label/">Label</a> | <a href="../irepd3axiszint/">3DAxisZ</a>.<a href="../../properties/irepd3axiszint-label/">Label</a> | <a href="../ireppolarradialaxisint/">PolarRadialAxis</a>.<a href="../../properties/ireppolarradialaxisint-label/">Label</a> | <a href="../irepspideraxisint/">SpiderAxis</a>.<a href="#" data-unresolved="1">Label</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepAxisLabelInt.htm`*
