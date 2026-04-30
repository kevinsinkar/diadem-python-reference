---
title: "IRepLabelRepetitionInt.PercentValue"
description: "Specifies the repetition of the curve labels as a percentage of the curve length in a 2D axis system in DIAdem REPORT."
---

# IRepLabelRepetitionInt.PercentValue

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: PercentValue for LabelRepetition

Specifies the repetition of the curve labels as a percentage of the curve length in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.PercentValue
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
oMyLabel.YValueFormat = "d.d"
oMyLabel.Position.Type = dd.e2DLabelPositionAtPoint
oMyLabel.Repetition.Mode = dd.eLabelRepetitionLength
oMyLabel.Repetition.PercentValue = 20
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_PercentValue_IRepLabelRepetitionInt.htm`*
