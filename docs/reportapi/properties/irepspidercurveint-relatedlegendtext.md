---
title: "IRepSpiderCurveInt.RelatedLegendText"
description: "Specifies the curve-related text of the legend of a spider axis system in DIAdem REPORT. To assign new text to the RelatedLegendText property in Python, use the"
---

# IRepSpiderCurveInt.RelatedLegendText

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelatedLegendText for SpiderCurve

Specifies the curve-related text of the legend of a spider axis system in DIAdem REPORT. To assign new text to the RelatedLegendText property in Python, use the syntax SetRelatedLegendText( Column , NewText ) .

## Signature

```python
obj.RelatedLegendText(Column)
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

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"
oMyCurve.Name = "MySpiderCurve"
oMyCurve.Enable = True

oMyAxisSystem.CurveLegend.Visible = True
oMyCurveLegendText = oMyAxisSystem.CurveLegend.Columns.Add()
oMyCurveLegendText.Type = dd.eLegendTextCurveRelatedText
oMyCurve.SetRelatedLegendText(2, "Spider Curve")

oMyLegendPosition = oMyAxisSystem.CurveLegend.Position
oMyLegendPosition.RelativePosition = dd.eLegendRelativePositionBottomRight
oMyLegendPosition.ElementHeight = 10
oMyLegendPosition.ElementWidth = 20

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RelatedLegendText_IRepSpiderCurveInt.htm`*
