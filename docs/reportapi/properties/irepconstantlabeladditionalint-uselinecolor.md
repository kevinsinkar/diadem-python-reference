---
title: "IRepConstantLabelAdditionalInt.UseLineColor"
description: "Specifies whether DIAdem REPORT displays the curve end label in 2D and 3D axis systems in the Constant display mode in the same color as the curve."
---

# IRepConstantLabelAdditionalInt.UseLineColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseLineColor for AdditionalConstantLabel

Specifies whether DIAdem REPORT displays the curve end label in 2D and 3D axis systems in the Constant display mode in the same color as the curve.

## Signature

```python
obj.UseLineColor
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseLineColor_IRepConstantLabelAdditionalInt.htm`*
