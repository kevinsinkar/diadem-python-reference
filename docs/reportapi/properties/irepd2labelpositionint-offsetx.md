---
title: "IRepD2LabelPositionInt.OffsetX"
description: "Specifies the fixed x-position of the curve label in relation to the axis origin in a 2D axis system in DIAdem REPORT."
---

# IRepD2LabelPositionInt.OffsetX

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OffsetX for 2DLabelPosition

Specifies the fixed x-position of the curve label in relation to the axis origin in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.OffsetX
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyLabel = oMyCurve.Shape.Extensions.Label
oMyLabel.YValueVisible = True
oMyLabel.YValueFormat = "d.dd"
oMyLabel.Repetition.Mode = dd.e2DLabelRepetitionMaxNPoints
oMyLabel.Repetition.NValue = 10
oMyLabel.Position.Type = dd.e2DLabelPositionFixedY
oMyLabel.Position.OffsetY = 15
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OffsetX_IRepD2LabelPositionInt.htm`*
