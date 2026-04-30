---
title: "IRepD2AxisXInt"
description: "The 2DAxisX object provides the properties of an x-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisXInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAxisX

The 2DAxisX object provides the properties of an x-axis in a 2D axis system in DIAdem REPORT.

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
<p><a href="../../properties/irepd2axisxint-disablecurveclipping/">DisableCurveClipping</a> | <a href="../../properties/irepd2axisxint-label/">Label</a> | <a href="../../properties/irepd2axisxint-line/">Line</a> | <a href="../../properties/irepd2axisxint-name/">Name</a> | <a href="../../properties/irepd2axisxint-numbers/">Numbers</a> | <a href="../../properties/irepd2axisxint-offsetorigin/">OffsetOrigin</a> | <a href="../../properties/irepd2axisxint-offsetvertical/">OffsetVertical</a> | <a href="../../properties/irepd2axisxint-scaling/">Scaling</a> | <a href="../../properties/irepd2axisxint-tagstored/">TagStored</a> | <a href="../../properties/irepd2axisxint-tagtemporary/">TagTemporary</a> | <a href="../../properties/irepd2axisxint-targetunit/">TargetUnit</a> | <a href="../../properties/irepd2axisxint-tickdisplay/">TickDisplay</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd2axisxint-convertpagexpositiontoxaxisvalue/">ConvertPageXPositionToXAxisValue</a> | <a href="../../methods/irepd2axisxint-convertxaxisvaluetopagexposition/">ConvertXAxisValueToPageXPosition</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisint/">2DAxisSystem</a>.<a href="../../properties/irepd2axisint-xaxis/">XAxis</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisXInt.htm`*
