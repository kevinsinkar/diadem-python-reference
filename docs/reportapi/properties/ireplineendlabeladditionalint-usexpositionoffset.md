---
title: "IRepLineEndLabelAdditionalInt.UseXPositionOffset"
description: "Specifies whether DIAdem REPORT plots the curve end labels at the x-value of the curve point or displaced to the x-value in a 2D axis system with the display mo"
---

# IRepLineEndLabelAdditionalInt.UseXPositionOffset

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseXPositionOffset for AdditionalLineEndLabel

Specifies whether DIAdem REPORT plots the curve end labels at the x-value of the curve point or displaced to the x-value in a 2D axis system with the display modes Line and points or Special combination .

## Signature

```python
obj.UseXPositionOffset
```

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
oMyEndLabel.UseXPositionOffset = False
oMyEndLabel.UseYPositionOffset = False
oMyEndLabel.Text = "End label"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseXPositionOffset_IRepLineEndLabelAdditionalInt.htm`*
