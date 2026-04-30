---
title: "IRepD2LabelAdditionalInt.Separator"
description: "Specifies the separator that DIAdem REPORT uses between the individual texts of the curve labels in a 2D axis system."
---

# IRepD2LabelAdditionalInt.Separator

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Separator for 2DAdditionalLabel

Specifies the separator that DIAdem REPORT uses between the individual texts of the curve labels in a 2D axis system.

## Signature

```python
obj.Separator
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLabelSeparatorSpace` | 0 | Spaces |
| `eLabelSeparatorComma` | 1 | Comma |
| `eLabelSeparatorSemicolon` | 2 | Semicolon |
| `eLabelSeparatorDot` | 3 | Point |

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
oMyLabel.XValueVisible = True
oMyLabel.XValueFormat = "d"
oMyLabel.Separator = dd.eLabelSeparatorSemicolon
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

*Source: `ReportApi/properties/Report_property_Separator_IRepD2LabelAdditionalInt.htm`*
