---
title: "IRepD2AxisInt.YAxisList"
description: "Specifies the collection of all 2DAxisY objects in DIAdem REPORT. The first object of the 2DAxisYAxisList collection is identical with the 2DAxisY object."
---

# IRepD2AxisInt.YAxisList

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YAxisList for 2DAxisSystem

Specifies the collection of all 2DAxisY objects in DIAdem REPORT. The first object of the 2DAxisYAxisList collection is identical with the 2DAxisY object.

## Signature

```python
return_value = obj.YAxisList
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMy2DCurve1 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyFirstCurve")
oMy2DCurve1.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve1.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve2 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MySecondCurve")
oMy2DCurve2.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve2.Shape.YChannel.Reference = "[1]/[3]"
oMyAxis = oMy2DaxisSystem.YAxisList.Add("SecondAxis")
oMy2DCurve2.YAxisReference = "SecondAxis"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<p class="body">The following example generates a 2D axis system with a curve and adds a further y-axis to the axis system:</p>
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p>
</div>
<div class="codeblue">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMy2DaxisSystem, oMyPosition, oMy2DCurve1, oMy2DCurve2, oMyAxis
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Data.Root.Clear</span>()
<span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">DataFileLoad</span>(<span class="Hldiademvariable">DataReadPath</span> &amp; <span class="HlString">"Example.tdm"</span>,<span class="HlString">"TDM"</span>,<span class="HlString">""</span>)
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.NewLayout</span>()
<span class="HlVBSKeyword">Set</span> oMy2DaxisSystem = <span class="Hldiademobject">Report.ActiveSheet.Objects.Add</span>(<span class="Hldiademconstant">eReportObject2DAxisSystem</span>,<span class="HlString">"My2DAxisSystem"</span>)
<span class="HlVBSKeyword">Set</span> oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = <span class="HlNumbers">20</span>
oMyPosition.Y1 = <span class="HlNumbers">20</span>
oMyPosition.X2 = <span class="HlNumbers">80</span>
oMyPosition.Y2 = <span class="HlNumbers">80</span>
<span class="HlVBSKeyword">Set</span> oMy2DCurve1 = oMy2DaxisSystem.Curves2D.Add(<span class="Hldiademconstant">e2DShapeLine</span>, <span class="HlString">"MyFirstCurve"</span>)
oMy2DCurve1.Shape.XChannel.Reference = <span class="HlString">"[1]/[1]"</span>
oMy2DCurve1.Shape.YChannel.Reference = <span class="HlString">"[1]/[2]"</span>
<span class="HlVBSKeyword">Set</span> oMy2DCurve2 = oMy2DaxisSystem.Curves2D.Add(<span class="Hldiademconstant">e2DShapeLine</span>, <span class="HlString">"MySecondCurve"</span>)
oMy2DCurve2.Shape.XChannel.Reference = <span class="HlString">"[1]/[1]"</span>
oMy2DCurve2.Shape.YChannel.Reference = <span class="HlString">"[1]/[3]"</span>
<span class="HlVBSKeyword">Set</span> oMyAxis = oMy2DaxisSystem.YAxisList.Add(<span class="HlString">"SecondAxis"</span>)
oMy2DCurve2.YAxisReference = <span class="HlString">"SecondAxis"</span>
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.Refresh</span>()</donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>dd.Data.Root.Clear() 
dd.DataFileLoad(dd.DataReadPath + <span class="HlString">"Example.tdm"</span>,<span class="HlString">"TDM"</span>,<span class="HlString">""</span>) 
dd.Report.NewLayout() 
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,<span class="HlString">"My2DAxisSystem"</span>) 
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate 
oMyPosition.X1 = <span class="HlNumbers">20</span> 
oMyPosition.Y1 = <span class="HlNumbers">20</span> 
oMyPosition.X2 = <span class="HlNumbers">80</span> 
oMyPosition.Y2 = <span class="HlNumbers">80</span> 
oMy2DCurve1 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, <span class="HlString">"MyFirstCurve"</span>) 
oMy2DCurve1.Shape.XChannel.Reference = <span class="HlString">"[1]/[1]"</span> 
oMy2DCurve1.Shape.YChannel.Reference = <span class="HlString">"[1]/[2]"</span> 
oMy2DCurve2 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, <span class="HlString">"MySecondCurve"</span>) 
oMy2DCurve2.Shape.XChannel.Reference = <span class="HlString">"[1]/[1]"</span> 
oMy2DCurve2.Shape.YChannel.Reference = <span class="HlString">"[1]/[3]"</span> 
oMyAxis = oMy2DaxisSystem.YAxisList.Add(<span class="HlString">"SecondAxis"</span>) 
oMy2DCurve2.YAxisReference = <span class="HlString">"SecondAxis"</span> 
dd.Report.Refresh() 
		 </donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YAxisList_IRepD2AxisInt.htm`*
