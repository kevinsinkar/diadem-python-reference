---
title: "IRepLabelNumericYInt"
description: "The LabelNumericY object provides the font attributes of a y-axis scale in DIAdem REPORT."
---

# IRepLabelNumericYInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: LabelNumericY

The LabelNumericY object provides the font attributes of a y-axis scale in DIAdem REPORT.

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
<p><a href="../../properties/ireplabelnumericyint-angle/">Angle</a> | <a href="../../properties/ireplabelnumericyint-font/">Font</a> | <a href="../../properties/ireplabelnumericyint-format/">Format</a> | <a href="../../properties/ireplabelnumericyint-relativeposition/">RelativePosition</a> | <a href="../../properties/ireplabelnumericyint-showendlabels/">ShowEndLabels</a> | <a href="../../properties/ireplabelnumericyint-textalignment/">TextAlignment</a> | <a href="../../properties/ireplabelnumericyint-usecurvecolor/">UseCurveColor</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisyint/">2DAxisY</a>.<a href="../../properties/irepd2axisyint-numbers/">Numbers</a></p></div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepLabelNumericYInt.htm`*
