---
title: "IRepCurveLegendInt.Header"
description: "Specifies the properties of the curve legend title in an axis system in DIAdem REPORT."
---

# IRepCurveLegendInt.Header

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Header for CurveLegend

Specifies the properties of the curve legend title in an axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Header
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = True
oMyAnchor = oMyLegend.Position.Anchor
oMyAnchor.PageRelatedX = 10
oMyAnchor.PageRelatedY = 10
oMyLegend.Columns(1).Title = "Legend Title"
oMyLegendHeader = oMyLegend.Header
oMyLegendHeader.ShowGrid = True
oMyLegendHeader.PortionHeaderField = 5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p>
</div>
<div class="codeblue" contenteditable="false">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMy2DAxisSystem, oMyPosition, oMyCurve, oMyShape, oMyLegend, oMyAnchor, oMyLegendHeader
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.NewLayout</span>()
<span class="HlVBSKeyword">Set</span> oMy2DAxisSystem = <span class="Hldiademobject">Report.ActiveSheet.Objects.Add</span>(<span class="Hldiademconstant">eReportObject2DAxisSystem</span>, <span class="HlString">"My2DAxisSystem"</span>)
<span class="HlVBSKeyword">Set</span> oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = <span class="HlNumbers">20</span>
oMyPosition.X2 = <span class="HlNumbers">80</span>
oMyPosition.Y1 = <span class="HlNumbers">20</span>
oMyPosition.Y2 = <span class="HlNumbers">80</span>
<span class="HlVBSKeyword">Set</span> oMyCurve = oMy2DAxisSystem.Curves2D.Add(<span class="Hldiademconstant">e2DShapeLine</span>, <span class="HlString">"MyNew2DCurve1"</span>)
oMyCurve.Shape.XChannel.Reference = <span class="HlString">"[1]/[1]"</span>
oMyCurve.Shape.YChannel.Reference = <span class="HlString">"[1]/[2]"</span>
<span class="HlVBSKeyword">Set</span> oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = <span class="HlVBSKeyword">True</span>
<span class="HlVBSKeyword">Set</span> oMyAnchor = oMyLegend.Position.Anchor
oMyAnchor.PageRelatedX = <span class="HlNumbers">10</span>
oMyAnchor.PageRelatedY = <span class="HlNumbers">10</span>
oMyLegend.Columns(<span class="HlNumbers">1</span>).Title = <span class="HlString">"Legend Title"</span>
<span class="HlVBSKeyword">Set</span> oMyLegendHeader = oMyLegend.Header
oMyLegendHeader.ShowGrid = <span class="HlVBSKeyword">True</span>
oMyLegendHeader.PortionHeaderField = <span class="HlNumbers">5</span>
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.Refresh</span>()</donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>dd.Report.NewLayout() 
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, <span class="HlString">"My2DAxisSystem"</span>) 
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate 
oMyPosition.X1 = <span class="HlNumbers">20</span> 
oMyPosition.X2 = <span class="HlNumbers">80</span> 
oMyPosition.Y1 = <span class="HlNumbers">20</span> 
oMyPosition.Y2 = <span class="HlNumbers">80</span> 
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, <span class="HlString">"MyNew2DCurve1"</span>) 
oMyCurve.Shape.XChannel.Reference = <span class="HlString">"[1]/[1]"</span> 
oMyCurve.Shape.YChannel.Reference = <span class="HlString">"[1]/[2]"</span> 
oMyLegend = oMy2DAxisSystem.CurveLegend 
oMyLegend.Visible = <span class="HlVBSKeyword">True</span> 
oMyAnchor = oMyLegend.Position.Anchor 
oMyAnchor.PageRelatedX = <span class="HlNumbers">10</span> 
oMyAnchor.PageRelatedY = <span class="HlNumbers">10</span> 
oMyLegend.Columns(<span class="HlNumbers">1</span>).Title = <span class="HlString">"Legend Title"</span> 
oMyLegendHeader = oMyLegend.Header 
oMyLegendHeader.ShowGrid = <span class="HlVBSKeyword">True</span> 
oMyLegendHeader.PortionHeaderField = <span class="HlNumbers">5</span> 
dd.Report.Refresh() 
	 </donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Header_IRepCurveLegendInt.htm`*
