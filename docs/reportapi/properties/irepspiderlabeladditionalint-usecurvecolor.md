---
title: "IRepSpiderLabelAdditionalInt.UseCurveColor"
description: "Specifies whether DIAdem REPORT also uses the line color of the curve for the symbols in a spider axis system."
---

# IRepSpiderLabelAdditionalInt.UseCurveColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseCurveColor for SpiderAdditionalLabel

Specifies whether DIAdem REPORT also uses the line color of the curve for the symbols in a spider axis system.

## Signature

```python
obj.UseCurveColor
```

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
oMyAddLabel.Angle = 0
oMyAddLabel.Font.Bold = True
oMyAddLabel.FromChannel.Visible = True
oMyAddLabel.FromChannel.Channel.Reference = "[5]/[1]"
oMyAddLabel.Font.Size = 1.5
oMyAddLabel.IndexValueVisible = True
oMyAddLabel.IndexValueFormat = "d.d"
oMyAddLabel.TextVisible = True
oMyAddLabel.Text = "MyCurve"
oMyAddLabel.Separator = dd.eLabelSeparatorComma
oMyAddLabel.UseCurveColor = True

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseCurveColor_IRepSpiderLabelAdditionalInt.htm`*
