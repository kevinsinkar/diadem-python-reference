---
title: "IRepPolarLabelAdditionalInt.Separator"
description: "Specifies the separator which DIAdem REPORT uses to combine the individual texts of the labels in a polar axis system in the display mode Line and Points ."
---

# IRepPolarLabelAdditionalInt.Separator

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Separator for PolarAdditionalLabel

Specifies the separator which DIAdem REPORT uses to combine the individual texts of the labels in a polar axis system in the display mode Line and Points .

## Signature

```python
obj.Separator
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLabelSeparatorSpace` | 0 | Blanks |
| `eLabelSeparatorComma` | 1 | Comma |
| `eLabelSeparatorSemicolon` | 2 | Semicolon |
| `eLabelSeparatorDot` | 3 | Point |

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyLabel = oMyCurve.Shape.Extensions.Label
oMyLabel.YValueVisible = True
oMyLabel.YValueFormat = "d.dd"
oMyLabel.XValueVisible = True
oMyLabel.XValueFormat = "d"
oMyRepetition = oMyLabel.Repetition
oMyRepetition.Mode = dd.eLabelRepetitionNthPoint
oMyRepetition.NValue = 100
oMyLabel.Separator = dd.eLabelSeparatorSemicolon
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Separator_IRepPolarLabelAdditionalInt.htm`*
