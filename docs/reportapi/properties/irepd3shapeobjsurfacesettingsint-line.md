---
title: "IRepD3ShapeObjSurfaceSettingsInt.Line"
description: "Specifies the properties of the curve line in the Surface display mode in a 3D axis system in DIAdem REPORT."
---

# IRepD3ShapeObjSurfaceSettingsInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for 3DSurfaceSettings

Specifies the properties of the curve line in the Surface display mode in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue )
oMySettings.Line.Width = dd.eLineWidth0100
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.dd"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 8
oMyLabel.Position.Type = dd.e3DLabelPositionAtPoint
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexRed)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p>
</div>
<div class="codeblue" contenteditable="false">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMy3DAxisSystem, oMy3DCurve, oMyPos, oMyShape, oMySettings, oMyLabel
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.NewLayout</span>()
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Data.Root.Clear</span>()
<span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">DataFileLoad</span>(<span class="Hldiademvariable">DataReadPath</span> &amp; <span class="HlString">"Report_Data.tdm"</span>,<span class="HlString">"TDM"</span>,<span class="HlString">""</span>)
<span class="HlVBSKeyword">Set</span> oMy3DAxisSystem = <span class="Hldiademobject">Report.ActiveSheet.Objects.Add</span>(<span class="Hldiademconstant">eReportObject3DAxisSystem</span>,<span class="HlString">"My3DAxisSystem"</span>)
<span class="HlVBSKeyword">Set</span> oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = <span class="HlNumbers">20</span>
oMyPos.X2 = <span class="HlNumbers">80</span>
oMyPos.Y1 = <span class="HlNumbers">20</span> 
oMyPos.Y2 = <span class="HlNumbers">80</span>
<span class="HlVBSKeyword">Set</span> oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(<span class="Hldiademconstant">e3DShapeSurface</span>, <span class="HlString">"MyNew3DCurve"</span>)
<span class="HlVBSKeyword">Set</span> oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = <span class="Hldiademconstant">e3DDataStructureMatrix</span>
oMyShape.XChannel.Reference = <span class="HlString">"[2]/[1]"</span>
oMyShape.YChannel.Reference = <span class="HlString">"[2]/[2]"</span>
oMyShape.ZChannel.Reference = <span class="HlString">"[2]/[3]"</span>
<span class="HlVBSKeyword">Set</span> oMySettings = oMyShape.Settings
<span class="HlVBSKeyword">Call</span> oMySettings.Line.Color.SetPredefinedColor(<span class="Hldiademconstant">eColorIndexBlue</span> )
oMySettings.Line.Width = <span class="Hldiademconstant">eLineWidth0100</span>
<span class="HlVBSKeyword">Set</span> oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = <span class="HlVBSKeyword">True</span>
oMyLabel.ZValueVisible = <span class="HlVBSKeyword">True</span>
oMyLabel.ZValueFormat = <span class="HlString">"d.dd"</span>
oMyLabel.Repetition.Mode = <span class="Hldiademconstant">e3DLabelRepetitionNthPoint</span>
oMyLabel.Repetition.NValue = <span class="HlNumbers">8</span>
oMyLabel.Position.Type = <span class="Hldiademconstant">e3DLabelPositionAtPoint</span>
<span class="HlVBSKeyword">Call</span> oMyLabel.Font.Color.SetPredefinedColor(<span class="Hldiademconstant">eColorIndexRed</span>)
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.Refresh</span>()</donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>dd.Report.NewLayout() 
dd.Data.Root.Clear() 
dd.DataFileLoad(dd.DataReadPath + <span class="HlString">"Report_Data.tdm"</span>,<span class="HlString">"TDM"</span>,<span class="HlString">""</span>) 
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,<span class="HlString">"My3DAxisSystem"</span>) 
oMyPos = oMy3DAxisSystem.Position.ByCoordinate 
oMyPos.X1 = <span class="HlNumbers">20</span> 
oMyPos.X2 = <span class="HlNumbers">80</span> 
oMyPos.Y1 = <span class="HlNumbers">20</span> 
oMyPos.Y2 = <span class="HlNumbers">80</span> 
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, <span class="HlString">"MyNew3DCurve"</span>) 
oMyShape = oMy3DCurve.Shape 
oMyShape.DataStructure = dd.e3DDataStructureMatrix 
oMyShape.XChannel.Reference = <span class="HlString">"[2]/[1]"</span> 
oMyShape.YChannel.Reference = <span class="HlString">"[2]/[2]"</span> 
oMyShape.ZChannel.Reference = <span class="HlString">"[2]/[3]"</span> 
oMySettings = oMyShape.Settings 
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue ) 
oMySettings.Line.Width = dd.eLineWidth0100 
oMyLabel = oMyShape.Extensions.Label 
oMyLabel.Visible = <span class="HlVBSKeyword">True</span> 
oMyLabel.ZValueVisible = <span class="HlVBSKeyword">True</span> 
oMyLabel.ZValueFormat = <span class="HlString">"d.dd"</span> 
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint 
oMyLabel.Repetition.NValue = <span class="HlNumbers">8</span> 
oMyLabel.Position.Type = dd.e3DLabelPositionAtPoint 
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexRed) 
dd.Report.Refresh() 
	 </donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepD3ShapeObjSurfaceSettingsInt.htm`*
