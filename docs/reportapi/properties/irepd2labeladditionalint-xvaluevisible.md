---
title: "IRepD2LabelAdditionalInt.XValueVisible"
description: "Specifies whether DIAdem REPORT writes the x-coordinates at the curve points in a 2D axis system."
---

# IRepD2LabelAdditionalInt.XValueVisible

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: XValueVisible for 2DAdditionalLabel

Specifies whether DIAdem REPORT writes the x-coordinates at the curve points in a 2D axis system.

## Signature

```python
obj.XValueVisible
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
oMyLabel.XValueVisible = True
oMyLabel.XValueFormat = "d.dd"
oMyLabel.YValueVisible = True
oMyLabel.YValueFormat = "d.dd"
oMyLabel.Separator = dd.eLabelSeparatorSemicolon
oMyLabel.Position.Type = dd.e2DLabelPositionAtPoint
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

*Source: `ReportApi/properties/Report_property_XValueVisible_IRepD2LabelAdditionalInt.htm`*
