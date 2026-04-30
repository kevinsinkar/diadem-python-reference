---
title: "IRepD3LabelIsolineAdditionalInt.Separator"
description: "Specifies the separator that DIAdem REPORT uses between individual texts in the isoline labels in a 3D display."
---

# IRepD3LabelIsolineAdditionalInt.Separator

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Separator for 3DAdditionalIsolineLabel

Specifies the separator that DIAdem REPORT uses between individual texts in the isoline labels in a 3D display.

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
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeIsolines, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[4]/[1]"
oMyShape.YChannel.Reference = "[4]/[2]"
oMyShape.NumberOfIsoChannels.Count = 3
oMyLabel = oMyShape.Extensions.IsolineLabel
oMyLabel.Visible = True
oMyLabel.TextVisible = True
oMyLabel.Text = "Z-Value"
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.d"
oMyLabel.Separator = dd.eLabelSeparatorSpace
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionLength
oMyLabel.Repetition.PercentValue = 30
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Separator_IRepD3LabelIsolineAdditionalInt.htm`*
