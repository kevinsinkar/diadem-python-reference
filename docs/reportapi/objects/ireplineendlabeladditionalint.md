---
title: "IRepLineEndLabelAdditionalInt"
description: "The AdditionalLineEndLabel object provides curve end labels in 2D axis systems in DIAdem REPORT."
---

# IRepLineEndLabelAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: AdditionalLineEndLabel

The AdditionalLineEndLabel object provides curve end labels in 2D axis systems in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyEndLabel = oMyCurve.Shape.Extensions.EndLabel
oMyEndLabel.Position = dd.e2DLineEndLabelPositionLargestXValue
oMyEndLabel.Type = dd.e2DLineEndLabelCustomText
oMyEndLabel.Text = "End label"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireplineendlabeladditionalint-angle/">Angle</a> | <a href="../../properties/ireplineendlabeladditionalint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/ireplineendlabeladditionalint-font/">Font</a> | <a href="../../properties/ireplineendlabeladditionalint-position/">Position</a> | <a href="../../properties/ireplineendlabeladditionalint-relativeposition/">RelativePosition</a> | <a href="../../properties/ireplineendlabeladditionalint-showatnovalues/">ShowAtNoValues</a> | <a href="../../properties/ireplineendlabeladditionalint-text/">Text</a> | <a href="../../properties/ireplineendlabeladditionalint-type/">Type</a> | <a href="../../properties/ireplineendlabeladditionalint-usecurvecolor/">UseCurveColor</a> | <a href="../../properties/ireplineendlabeladditionalint-uselabelonlyonfirstexpandedcurve/">UseLabelOnlyOnFirstExpandedCurve</a> | <a href="../../properties/ireplineendlabeladditionalint-usexpositionoffset/">UseXPositionOffset</a> | <a href="../../properties/ireplineendlabeladditionalint-useypositionoffset/">UseYPositionOffset</a> | <a href="../../properties/ireplineendlabeladditionalint-xpositionoffset/">XPositionOffset</a> | <a href="../../properties/ireplineendlabeladditionalint-ypositionoffset/">YPositionOffset</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjlineandpointsextensionsint/">2DLineAndPointsExtensions</a>.<a href="../../properties/irepd2shapeobjlineandpointsextensionsint-endlabel/">EndLabel</a> | <a href="../irepd2shapeobjspecialcombinationextensionsint/">2DSpecialCombinationExtensions</a>.<a href="../../properties/irepd2shapeobjspecialcombinationextensionsint-endlabel/">EndLabel</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepLineEndLabelAdditionalInt.htm`*
