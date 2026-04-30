---
title: "IRepD2SpecialCombAdditionalStylesInt.Line"
description: "Specifies the line properties of a curve in the Special combination display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2SpecialCombAdditionalStylesInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for 2DAdditionalStyles

Specifies the line properties of a curve in the Special combination display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyAdditionalStyles = oMyShape.Extensions.AdditionalStyles
oMyAdditionalStyles.Type = dd.e2DAdditionalStyleSpikes
oMyAdditionalStyles.Line.Color.SetPredefinedColor(dd.eColorIndexRed)
oMyAdditionalStyles.Line.Width = dd.eLineWidth0025
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p>
</div>
<div class="codeblue" contenteditable="false">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMy2DAxisSystem, oMyCurve, oMyPos, oMyShape, oMySetting, oMyAdditionalStyles
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Data.Root.Clear</span>()
<span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">DataFileLoad</span>(<span class="Hldiademvariable">DataReadPath</span> &amp; <span class="HlString">"Report_Data.tdm"</span>,<span class="HlString">"TDM"</span>,<span class="HlString">""</span>)
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.NewLayout</span>()
<span class="HlVBSKeyword">Set</span> oMy2DAxisSystem = <span class="Hldiademobject">Report.ActiveSheet.Objects.Add</span>(<span class="Hldiademconstant">eReportObject2DAxisSystem</span>, <span class="HlString">"My2DAxisSystem"</span>)
<span class="HlVBSKeyword">Set</span> oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = <span class="HlNumbers">20</span>
oMyPos.X2 = <span class="HlNumbers">80</span>
oMyPos.Y1 = <span class="HlNumbers">20</span>
oMyPos.Y2 = <span class="HlNumbers">80</span>
<span class="HlVBSKeyword">Set</span> oMyCurve = oMy2DAxisSystem.Curves2D.Add(<span class="Hldiademconstant">e2DShapeSpecialCombination</span>, <span class="HlString">"MyCurve"</span>)
<span class="HlVBSKeyword">Set</span> oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = <span class="HlString">"[6]/[1]"</span> 
oMyShape.YChannel.Reference = <span class="HlString">"[6]/[2]"</span> 
<span class="HlVBSKeyword">Set</span> oMySetting = oMyShape.Settings
<span class="HlVBSKeyword">Call</span> oMySetting.Line.Color.SetPredefinedColor(<span class="Hldiademconstant">eColorIndexBlue</span>)
oMySetting.Line.Width = <span class="Hldiademconstant">eLineWidth0100</span>
<span class="HlVBSKeyword">Set</span> oMyAdditionalStyles = oMyShape.Extensions.AdditionalStyles
oMyAdditionalStyles.Type = <span class="Hldiademconstant">e2DAdditionalStyleSpikes</span>
<span class="HlVBSKeyword">Call</span> oMyAdditionalStyles.Line.Color.SetPredefinedColor(<span class="Hldiademconstant">eColorIndexRed</span>)
oMyAdditionalStyles.Line.Width = <span class="Hldiademconstant">eLineWidth0025</span>
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.Refresh</span>()</donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>dd.Data.Root.Clear() 
dd.DataFileLoad(dd.DataReadPath + <span class="HlString">"Report_Data.tdm"</span>,<span class="HlString">"TDM"</span>,<span class="HlString">""</span>) 
dd.Report.NewLayout() 
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, <span class="HlString">"My2DAxisSystem"</span>) 
oMyPos = oMy2DAxisSystem.Position.ByCoordinate 
oMyPos.X1 = <span class="HlNumbers">20</span> 
oMyPos.X2 = <span class="HlNumbers">80</span> 
oMyPos.Y1 = <span class="HlNumbers">20</span> 
oMyPos.Y2 = <span class="HlNumbers">80</span> 
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, <span class="HlString">"MyCurve"</span>) 
oMyShape = oMyCurve.Shape 
oMyShape.XChannel.Reference = <span class="HlString">"[6]/[1]"</span> 
oMyShape.YChannel.Reference = <span class="HlString">"[6]/[2]"</span> 
oMySetting = oMyShape.Settings 
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue) 
oMySetting.Line.Width = dd.eLineWidth0100 
oMyAdditionalStyles = oMyShape.Extensions.AdditionalStyles 
oMyAdditionalStyles.Type = dd.e2DAdditionalStyleSpikes 
oMyAdditionalStyles.Line.Color.SetPredefinedColor(dd.eColorIndexRed) 
oMyAdditionalStyles.Line.Width = dd.eLineWidth0025 
dd.Report.Refresh() 
	 </donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepD2SpecialCombAdditionalStylesInt.htm`*
