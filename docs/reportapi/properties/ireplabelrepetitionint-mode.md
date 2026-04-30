---
title: "IRepLabelRepetitionInt.Mode"
description: "Specifies how DIAdem REPORT repeats the curve labels in a 2D axis system."
---

# IRepLabelRepetitionInt.Mode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Mode for LabelRepetition

Specifies how DIAdem REPORT repeats the curve labels in a 2D axis system.

## Signature

```python
obj.Mode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLabelRepetitionEveryPoint` | 0 | Every point |
| `eLabelRepetitionNthPoint` | 1 | Every n points |
| `eLabelRepetitionMaxNPoints` | 2 | Maximum n points |
| `eLabelRepetitionLength` | 3 | Every n percent |

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
oMyLabel.Repetition.Mode = dd.eLabelRepetitionMaxNPoints
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

*Source: `ReportApi/properties/Report_property_Mode_IRepLabelRepetitionInt.htm`*
