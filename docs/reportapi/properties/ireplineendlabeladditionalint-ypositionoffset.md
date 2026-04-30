---
title: "IRepLineEndLabelAdditionalInt.YPositionOffset"
description: "Specifies the vertical offset of the curve end label as a percentage in a 2D axis system in DIAdem REPORT."
---

# IRepLineEndLabelAdditionalInt.YPositionOffset

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YPositionOffset for AdditionalLineEndLabel

Specifies the vertical offset of the curve end label as a percentage in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.YPositionOffset
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
oMyEndLabel.Position = dd.e2DLineEndLabelPositionLargestIndex
oMyEndLabel.Type = dd.e2DLineEndLabelCustomText
oMyEndLabel.Text = "End label"
oMyEndLabel.UseXPositionOffset = True
oMyEndLabel.XPositionOffset = 5
oMyEndLabel.UseYPositionOffset = True
oMyEndLabel.YPositionOffset = 5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YPositionOffset_IRepLineEndLabelAdditionalInt.htm`*
