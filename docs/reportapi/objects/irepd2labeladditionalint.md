---
title: "IRepD2LabelAdditionalInt"
description: "The 2DAdditionalLabel object provides the label properties for a 2D curve in the display modes Line and points or Special combination in DIAdem REPORT."
---

# IRepD2LabelAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAdditionalLabel

The 2DAdditionalLabel object provides the label properties for a 2D curve in the display modes Line and points or Special combination in DIAdem REPORT.

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
oMyLabel.Repetition.Mode = dd.e2DLabelRepetitionMaxNPoints
oMyLabel.Repetition.NValue = 10
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2labeladditionalint-angle/">Angle</a> | <a href="../../properties/irepd2labeladditionalint-font/">Font</a> | <a href="../../properties/irepd2labeladditionalint-fromchannel/">FromChannel</a> | <a href="../../properties/irepd2labeladditionalint-indexvalueformat/">IndexValueFormat</a> | <a href="../../properties/irepd2labeladditionalint-indexvaluevisible/">IndexValueVisible</a> | <a href="../../properties/irepd2labeladditionalint-position/">Position</a> | <a href="../../properties/irepd2labeladditionalint-relativeposition/">RelativePosition</a> | <a href="../../properties/irepd2labeladditionalint-repetition/">Repetition</a> | <a href="../../properties/irepd2labeladditionalint-separator/">Separator</a> | <a href="../../properties/irepd2labeladditionalint-text/">Text</a> | <a href="../../properties/irepd2labeladditionalint-textvisible/">TextVisible</a> | <a href="../../properties/irepd2labeladditionalint-usecurvecolor/">UseCurveColor</a> | <a href="../../properties/irepd2labeladditionalint-uselabelonlyonfirstexpandedcurve/">UseLabelOnlyOnFirstExpandedCurve</a> | <a href="../../properties/irepd2labeladditionalint-xvalueformat/">XValueFormat</a> | <a href="../../properties/irepd2labeladditionalint-xvaluevisible/">XValueVisible</a> | <a href="../../properties/irepd2labeladditionalint-yvalueformat/">YValueFormat</a> | <a href="../../properties/irepd2labeladditionalint-yvaluevisible/">YValueVisible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjbarsextensionsint/">2DBarsExtensions</a>.<a href="../../properties/irepd2shapeobjbarsextensionsint-label/">Label</a> | <a href="../irepd2shapeobjlineandpointsextensionsint/">2DLineAndPointsExtensions</a>.<a href="../../properties/irepd2shapeobjlineandpointsextensionsint-label/">Label</a> | <a href="../irepd2shapeobjspecialcombinationextensionsint/">2DSpecialCombinationExtensions</a>.<a href="../../properties/irepd2shapeobjspecialcombinationextensionsint-label/">Label</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2LabelAdditionalInt.htm`*
