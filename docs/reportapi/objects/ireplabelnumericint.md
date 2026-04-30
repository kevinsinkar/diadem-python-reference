---
title: "IRepLabelNumericInt"
description: "The LabelNumeric object provides the font attributes of an axis scale in DIAdem REPORT."
---

# IRepLabelNumericInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: LabelNumeric

The LabelNumeric object provides the font attributes of an axis scale in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyXNumericLabel = oMy2DAxisSystem.XAxis.Numbers
oMyXNumericLabel.UseCurveColor = True
oMyXNumericLabel.Format = "#nn:ss"
oMyXNumericLabel.Angle = 90
oMyXNumericLabel.Font.Name = "Tahoma"
oMyXNumericLabel.Font.Size = 3
oMyXNumericLabel.RelativePosition = dd.eRelativePositionLeft
oMyYNumericLabel = oMy2DAxisSystem.YAxis.Numbers
oMyYNumericLabel.UseCurveColor = True
oMyYNumericLabel.Format = "d.dde"
oMyYNumericLabel.Angle = 0
oMyYNumericLabel.Font.Name = "Tahoma"
oMyYNumericLabel.Font.Size = 3
oMyYNumericLabel.RelativePosition = dd.eRelativePositionLeft
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireplabelnumericint-angle/">Angle</a> | <a href="../../properties/ireplabelnumericint-font/">Font</a> | <a href="../../properties/ireplabelnumericint-format/">Format</a> | <a href="../../properties/ireplabelnumericint-relativeposition/">RelativePosition</a> | <a href="../../properties/ireplabelnumericint-showendlabels/">ShowEndLabels</a> | <a href="../../properties/ireplabelnumericint-usecurvecolor/">UseCurveColor</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisxint/">2DAxisX</a>.<a href="../../properties/irepd2axisxint-numbers/">Numbers</a> | <a href="../irepd3axisxint/">3DAxisX</a>.<a href="../../properties/irepd3axisxint-numbers/">Numbers</a> | <a href="../irepd3axisyint/">3DAxisY</a>.<a href="../../properties/irepd3axisyint-numbers/">Numbers</a> | <a href="../irepd3axiszint/">3DAxisZ</a>.<a href="../../properties/irepd3axiszint-numbers/">Numbers</a> | <a href="../ireppolarradialaxisint/">PolarRadialAxis</a>.<a href="../../properties/ireppolarradialaxisint-numbers/">Numbers</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepLabelNumericInt.htm`*
