---
title: "IRepPolarShapeObjBaseInt.XChannel"
description: "Specifies the x-channel of a curve in a polar axis system in DIAdem REPORT."
---

# IRepPolarShapeObjBaseInt.XChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: XChannel for PolarShapeObject

Specifies the x-channel of a curve in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.XChannel
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,"MyPolarSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p>
</div>
<div class="codeblue">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMyPolarAxisSystem, oMyPosition, oMyCurve
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Data.Root.Clear</span>()
<span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">DataFileLoad</span>(<span class="Hldiademvariable">DataReadPath</span> &amp; <span class="HlString">"Report_Data.tdm"</span>,<span class="HlString">"TDM"</span>,<span class="HlString">""</span>)
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.NewLayout</span>()
<span class="HlVBSKeyword">Set</span> oMyPolarAxisSystem = <span class="Hldiademobject">Report.ActiveSheet.Objects.Add</span>(<span class="Hldiademconstant">eReportObjectPolarSystem</span>,<span class="HlString">"MyPolarSystem"</span>)
<span class="HlVBSKeyword">Set</span> oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = <span class="HlNumbers">20</span>
oMyPosition.Y1 = <span class="HlNumbers">20</span>
oMyPosition.X2 = <span class="HlNumbers">80</span>
oMyPosition.Y2 = <span class="HlNumbers">80</span>
<span class="HlVBSKeyword">Set</span> oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(<span class="Hldiademconstant">ePolarShapeLineAndPoints</span>, <span class="HlString">"MyNewCurve"</span>)
oMyCurve.Shape.XChannel.Reference = <span class="HlString">"[5]/[1]"</span>
oMyCurve.Shape.YChannel.Reference = <span class="HlString">"[5]/[2]"</span>
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.Refresh</span>()</donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>dd.Data.Root.Clear() 
dd.DataFileLoad(dd.DataReadPath + <span class="HlString">"Report_Data.tdm"</span>,<span class="HlString">"TDM"</span>,<span class="HlString">""</span>) 
dd.Report.NewLayout() 
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,<span class="HlString">"MyPolarSystem"</span>) 
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate 
oMyPosition.X1 = <span class="HlNumbers">20</span> 
oMyPosition.Y1 = <span class="HlNumbers">20</span> 
oMyPosition.X2 = <span class="HlNumbers">80</span> 
oMyPosition.Y2 = <span class="HlNumbers">80</span> 
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, <span class="HlString">"MyNewCurve"</span>) 
oMyCurve.Shape.XChannel.Reference = <span class="HlString">"[5]/[1]"</span> 
oMyCurve.Shape.YChannel.Reference = <span class="HlString">"[5]/[2]"</span> 
dd.Report.Refresh() 
	 </donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_XChannel_IRepPolarShapeObjBaseInt.htm`*
