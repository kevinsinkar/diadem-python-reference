---
title: "IRepLabelNumericInt.UseCurveColor"
description: "Specifies whether DIAdem REPORT also uses the curve color for the scale labels."
---

# IRepLabelNumericInt.UseCurveColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseCurveColor for LabelNumeric

Specifies whether DIAdem REPORT also uses the curve color for the scale labels.

## Signature

```python
obj.UseCurveColor
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyXNumericLabel = oMy2DAxisSystem.XAxis.Numbers
oMyXNumericLabel.UseCurveColor = True
oMyXNumericLabel.Format = "d.dde"
oMyXNumericLabel.Angle = 90
oMyXNumericLabel.Font.Name = "Tahoma"
oMyXNumericLabel.Font.Size = 3
oMyXNumericLabel.RelativePosition = dd.eRelativePositionLeft
oMyYNumericLabel = oMy2DAxisSystem.YAxis.Numbers
oMyYNumericLabel.UseCurveColor = True
oMyYNumericLabel.Format = "d.dde"
oMyYNumericLabel.Angle = 0
oMyYNumericLabel.Font.Name = "Tahoma"
oMyYNumericLabel.Font.Size = 3
oMyYNumericLabel.RelativePosition = dd.eRelativePositionLeft
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseCurveColor_IRepLabelNumericInt.htm`*
