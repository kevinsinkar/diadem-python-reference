---
title: "IRepConstantLabelAdditionalInt"
description: "The AdditionalConstantLabel object provides the properties of the constant labels in a 2D axis system in the Constant display mode in DIAdem REPORT."
---

# IRepConstantLabelAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: AdditionalConstantLabel

The AdditionalConstantLabel object provides the properties of the constant labels in a 2D axis system in the Constant display mode in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurveLine.Shape.XChannel.Reference = "[1]/[1]"
oMyCurveLine.Shape.YChannel.Reference = "[1]/[2]"
oMyCurveConst = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeConstant, "MyConstant")
oMyCurveConst.Shape.XConstant.Reference = 10
oMyCurveConst.Shape.YConstant.Reference = 20
oMyConstLabel = oMyCurveConst.Shape.Extensions.ConstantLabel
oMyConstLabel.Type = dd.e2DLabelValue
oMyConstLabel.UseLineColor = False
oMyConstLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlack )
oMyConstLabel.UseXPositionOffset = True
oMyConstLabel.UseYPositionOffset = True
oMyConstLabel.XPositionOffset = 5
oMyConstLabel.YPositionOffset = 5
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepconstantlabeladditionalint-angle/">Angle</a> | <a href="../../properties/irepconstantlabeladditionalint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/irepconstantlabeladditionalint-font/">Font</a> | <a href="../../properties/irepconstantlabeladditionalint-position/">Position</a> | <a href="../../properties/irepconstantlabeladditionalint-relativeposition/">RelativePosition</a> | <a href="../../properties/irepconstantlabeladditionalint-text/">Text</a> | <a href="../../properties/irepconstantlabeladditionalint-type/">Type</a> | <a href="../../properties/irepconstantlabeladditionalint-uselinecolor/">UseLineColor</a> | <a href="../../properties/irepconstantlabeladditionalint-usexpositionoffset/">UseXPositionOffset</a> | <a href="../../properties/irepconstantlabeladditionalint-useypositionoffset/">UseYPositionOffset</a> | <a href="../../properties/irepconstantlabeladditionalint-xpositionoffset/">XPositionOffset</a> | <a href="../../properties/irepconstantlabeladditionalint-ypositionoffset/">YPositionOffset</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjconstantextensionsint/">2DConstantExtensions</a>.<a href="../../properties/irepd2shapeobjconstantextensionsint-constantlabel/">ConstantLabel</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepConstantLabelAdditionalInt.htm`*
