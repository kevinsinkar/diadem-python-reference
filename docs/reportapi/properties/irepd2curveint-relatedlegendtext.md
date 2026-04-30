---
title: "IRepD2CurveInt.RelatedLegendText"
description: "Specifies the curve-related text in a 2D axis system legend in DIAdem REPORT. To assign new text to the RelatedLegendText property in Python, use the syntax Set"
---

# IRepD2CurveInt.RelatedLegendText

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelatedLegendText for 2DCurve

Specifies the curve-related text in a 2D axis system legend in DIAdem REPORT. To assign new text to the RelatedLegendText property in Python, use the syntax SetRelatedLegendText( Column , NewText ) .

## Signature

```python
obj.RelatedLegendText(Column)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve1 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "My2DCurve1")
oMy2DCurve1.Shape.XChannel.Reference = ""
oMy2DCurve1.Shape.YChannel.Reference = "[4]/[1]"
oMy2DCurve2 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "My2DCurve2")
oMy2DCurve2.Shape.XChannel.Reference = ""
oMy2DCurve2.Shape.YChannel.Reference = "[4]/[2]"
oMy2DAxisSystem.CurveLegend.Visible = True
oMyCurveLegendText = oMy2DAxisSystem.CurveLegend.Columns.Add()
oMyCurveLegendText.Type = dd.eLegendTextCurveRelatedText
oMy2DCurve1.SetRelatedLegendText(2, "First Curve")
oMy2DCurve2.SetRelatedLegendText(2, "Second Curve")
oMyLegendPosition = oMy2DAxisSystem.CurveLegend.Position
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

*Source: `ReportApi/properties/Report_property_RelatedLegendText_IRepD2CurveInt.htm`*
