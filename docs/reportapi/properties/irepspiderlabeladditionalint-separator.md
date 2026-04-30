---
title: "IRepSpiderLabelAdditionalInt.Separator"
description: "Specifies the separator with which DIAdem REPORT combines the individual texts of the labels in a spider axis system in the display mode Line and points ."
---

# IRepSpiderLabelAdditionalInt.Separator

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Separator for SpiderAdditionalLabel

Specifies the separator with which DIAdem REPORT combines the individual texts of the labels in a spider axis system in the display mode Line and points .

## Signature

```python
obj.Separator
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLabelSeparatorSpace` | 0 | Blank |
| `eLabelSeparatorComma` | 1 | Comma |
| `eLabelSeparatorSemicolon` | 2 | Semicolon |
| `eLabelSeparatorDot` | 3 | Point |

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLineAndPoints, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyAddLabel = oMyCurve.Shape.Extensions.Label
oMyAddLabel.Font.Size = 1.5
oMyAddLabel.ValueVisible = True
oMyAddLabel.ValueFormat = "d"
oMyAddLabel.Separator = dd.eLabelSeparatorComma

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Separator_IRepSpiderLabelAdditionalInt.htm`*
