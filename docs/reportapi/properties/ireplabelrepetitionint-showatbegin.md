---
title: "IRepLabelRepetitionInt.ShowAtBegin"
description: "Specifies whether DIAdem REPORT displays the curve label at the beginning of the curve in a 2D axis system."
---

# IRepLabelRepetitionInt.ShowAtBegin

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowAtBegin for LabelRepetition

Specifies whether DIAdem REPORT displays the curve label at the beginning of the curve in a 2D axis system.

## Signature

```python
obj.ShowAtBegin
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
oMyLabel.Repetition.PercentValue = 25
oMyLabel.Repetition.ShowAtBegin = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowAtBegin_IRepLabelRepetitionInt.htm`*
