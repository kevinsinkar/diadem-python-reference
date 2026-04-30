---
title: "IRepLabelRepetitionInt"
description: "The 2DLabelRepetition object provides the properties of the label repetitions for a 2D curve in the display modes Line and points or Special combination in DIAd"
---

# IRepLabelRepetitionInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: LabelRepetition

The 2DLabelRepetition object provides the properties of the label repetitions for a 2D curve in the display modes Line and points or Special combination in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyLabel = oMyCurve.Shape.Extensions.Label
oMyLabel.YValueVisible = True
oMyLabel.YValueFormat = "d.dd"
oMyLabel.Position.Type = dd.e2DLabelPositionAtPoint
oMyLabel.Repetition.Mode = dd.eLabelRepetitionMaxNPoints
oMyLabel.Repetition.NValue = 10
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireplabelrepetitionint-mode/">Mode</a> | <a href="../../properties/ireplabelrepetitionint-nvalue/">NValue</a> | <a href="../../properties/ireplabelrepetitionint-percentvalue/">PercentValue</a> | <a href="../../properties/ireplabelrepetitionint-showatbegin/">ShowAtBegin</a> | <a href="../../properties/ireplabelrepetitionint-showatend/">ShowAtEnd</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2labeladditionalint/">2DAdditionalLabel</a>.<a href="../../properties/irepd2labeladditionalint-repetition/">Repetition</a> | <a href="../ireppolarlabeladditionalint/">PolarAdditionalLabel</a>.<a href="../../properties/ireppolarlabeladditionalint-repetition/">Repetition</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepLabelRepetitionInt.htm`*
