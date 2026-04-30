---
title: "IRepD2LabelAdditionalInt.Text"
description: "Specifies the symbols or texts which DIAdem REPORT uses to mark the curve points in a 2D axis system."
---

# IRepD2LabelAdditionalInt.Text

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Text for 2DAdditionalLabel

Specifies the symbols or texts which DIAdem REPORT uses to mark the curve points in a 2D axis system.

## Signature

```python
obj.Text
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
oMyLabel.Position.Type = dd.e2DLabelPositionAtPoint
oMyLabel.Repetition.Mode = dd.e2DLabelRepetitionMaxNPoints
oMyLabel.Repetition.NValue = 10
oMyLabel.TextVisible = True
oMyLabel.Text = "*"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Text_IRepD2LabelAdditionalInt.htm`*
