---
title: "IRepD2LabelAdditionalInt.Angle"
description: "Specifies the text direction of the symbols in the display modes Line and points or Special combination in a 2D axis system in DIAdem-REPORT."
---

# IRepD2LabelAdditionalInt.Angle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Angle for 2DAdditionalLabel

Specifies the text direction of the symbols in the display modes Line and points or Special combination in a 2D axis system in DIAdem-REPORT.

## Signature

```python
obj.Angle
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you assign the value NoValue to the <span class="Monospace">Angle</span> property, DIAdem adapts the text angle automatically to the slope of the curve at the point to which the text is assigned.</td></tr></table>
</div>

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
oMyLabel.Repetition.Mode = dd.e2DLabelRepetitionMaxNPoints
oMyLabel.Repetition.NValue = 10
oMyLabel.Angle = 45
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Angle_IRepD2LabelAdditionalInt.htm`*
