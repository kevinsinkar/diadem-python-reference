---
title: "IRepD3CurveInt.RelatedLegendText"
description: "Specifies the curve-related text in a 3D axis system legend in DIAdem REPORT. To assign new text to the RelatedLegendText property in Python, use the syntax Set"
---

# IRepD3CurveInt.RelatedLegendText

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelatedLegendText for 3DCurve

Specifies the curve-related text in a 3D axis system legend in DIAdem REPORT. To assign new text to the RelatedLegendText property in Python, use the syntax SetRelatedLegendText( Column , NewText ) .

## Signature

```python
obj.RelatedLegendText(Column)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem, "My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve1 = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeBars, "My3DCurve1")
oMy3DCurve1.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve1.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve1.Shape.ZChannel.Reference = "[2]/[3]"
oMy3DCurve2 = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeLine, "My3DCurve2")
oMy3DCurve2.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve2.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve2.Shape.ZChannel.Reference = "[2]/[3]"
oMy3DAxisSystem.CurveLegend.Visible = True
oMyCurveLegendText = oMy3DAxisSystem.CurveLegend.Columns.Add()
oMyCurveLegendText.Type = dd.eLegendTextCurveRelatedText
oMy3DCurve1.SetRelatedLegendText(2, "First Curve")
oMy3DCurve2.SetRelatedLegendText(2, "Second Curve")
oMyLegendPosition = oMy3DAxisSystem.CurveLegend.Position
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

*Source: `ReportApi/properties/Report_property_RelatedLegendText_IRepD3CurveInt.htm`*
