---
title: "IRepConstantLabelAdditionalInt.RelativePosition"
description: "Specifies the relative position of the curve end label to the curve in a 2D axis system in DIAdem REPORT."
---

# IRepConstantLabelAdditionalInt.RelativePosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativePosition for AdditionalConstantLabel

Specifies the relative position of the curve end label to the curve in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.RelativePosition
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eRelativePositionRightTop` | 0 | Top right |
| `eRelativePositionCenter` | 1 | Center |
| `eRelativePositionRight` | 2 | Right |
| `eRelativePositionRightBottom` | 3 | Bottom right |
| `eRelativePositionTop` | 4 | Top |
| `eRelativePositionBottom` | 5 | Bottom |
| `eRelativePositionLeftTop` | 6 | Top left |
| `eRelativePositionLeft` | 7 | Left |
| `eRelativePositionLeftBottom` | 8 | Bottom left |

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
oMyConstLabel.RelativePosition = dd.eRelativePositionLeft
oMyConstLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlack)
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

*Source: `ReportApi/properties/Report_property_RelativePosition_IRepConstantLabelAdditionalInt.htm`*
