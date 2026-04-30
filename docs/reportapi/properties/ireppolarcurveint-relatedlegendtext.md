---
title: "IRepPolarCurveInt.RelatedLegendText"
description: "Specifies the curve-related text of the legend of a polar axis system in DIAdem REPORT. To assign new text to the RelatedLegendText property in Python, use the "
---

# IRepPolarCurveInt.RelatedLegendText

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelatedLegendText for PolarCurve

Specifies the curve-related text of the legend of a polar axis system in DIAdem REPORT. To assign new text to the RelatedLegendText property in Python, use the syntax SetRelatedLegendText( Column , NewText ) .

## Signature

```python
obj.RelatedLegendText(Column)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarSystem")
oMyPolarCurve = oMyPolarSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyPolarCurve")
oMyPolarCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyPolarCurve.Shape.YChannel.Reference = "[5]/[2]"

oMyPolarSystem.CurveLegend.Visible = True
oMyPolarSystem.CurveLegend.Columns(1).Type = dd.eLegendTextCurveRelatedText
oMyPolarCurve.SetRelatedLegendText(1, "Polar data")
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RelatedLegendText_IRepPolarCurveInt.htm`*
