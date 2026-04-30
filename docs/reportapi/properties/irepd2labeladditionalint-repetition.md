---
title: "IRepD2LabelAdditionalInt.Repetition"
description: "Specifies how DIAdem REPORT repeats the curve labels in a 2D axis system. If you set Every n percent , DIAdem REPORT first specifies the distance that correspon"
---

# IRepD2LabelAdditionalInt.Repetition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Repetition for 2DAdditionalLabel

Specifies how DIAdem REPORT repeats the curve labels in a 2D axis system. If you set Every n percent , DIAdem REPORT first specifies the distance that corresponds with the percentage value of the diagonal of the diagram area. DIAdem applies this distance along the curve and plots the labels at the next point.

## Signature

```python
return_value = obj.Repetition
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
oMyLabel.Position.Type = dd.e2DLabelPositionAtPoint
oMyLabel.RelativePosition = dd.eRelativePositionLeft
oMyLabel.Repetition.Mode = dd.e2DLabelRepetitionMaxNPoints
oMyLabel.Repetition.NValue = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Repetition_IRepD2LabelAdditionalInt.htm`*
