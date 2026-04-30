---
title: "IRepD2AxisXScalingInt.Origin"
description: "Specifies the value at which the vertical axis intersects the selected axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisXScalingInt.Origin

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Origin for 2DAxisXScaling

Specifies the value at which the vertical axis intersects the selected axis in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Origin
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyXScaling = oMy2DAxisSystem.XAxis.Scaling
oMyXScaling.AutoScalingType = dd.eAxisAutoScalingManual
oMyXScaling.Type = dd.e2DXScalingLogarithmic
oMyXScaling.Begin = 0.01
oMyXScaling.End = 100
oMyXScaling.Origin = 1
oMyXScaling.Tick.Distance = 1
oMyXScaling.MiniTickCount = 10
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling
oMyYScaling.AutoScalingType = dd.eAxisAutoScalingManual
oMyYScaling.Type = dd.e2DYScalingLinear
oMyYScaling.Begin = 0
oMyYScaling.End = 100
oMyYScaling.Origin = 50
oMyYScaling.Tick.Distance = 12.5
oMyYScaling.MiniTickCount = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p>
</div>
<div class="codeblue" contenteditable="false">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMy2DAxisSystem, oMyPos, oMyXScaling, oMyYScaling
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.NewLayout</span>()
<span class="HlVBSKeyword">Set</span> oMy2DAxisSystem = <span class="Hldiademobject">Report.ActiveSheet.Objects.Add</span>(<span class="Hldiademconstant">eReportObject2DAxisSystem</span>, <span class="HlString">"My2DAxisSystem"</span>)
<span class="HlVBSKeyword">Set</span> oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = <span class="HlNumbers">20</span>
oMyPos.X2 = <span class="HlNumbers">80</span>
oMyPos.Y1 = <span class="HlNumbers">20</span>
oMyPos.Y2 = <span class="HlNumbers">80</span>
<span class="HlVBSKeyword">Set</span> oMyXScaling = oMy2DAxisSystem.XAxis.Scaling
oMyXScaling.AutoScalingType = <span class="Hldiademconstant">eAxisAutoScalingManual</span>
oMyXScaling.Type = <span class="Hldiademconstant">e2DXScalingLogarithmic</span>
oMyXScaling.Begin = <span class="HlNumbers">0</span>.<span class="HlNumbers">01</span>
oMyXScaling.End = <span class="HlNumbers">100</span>
oMyXScaling.Origin = <span class="HlNumbers">1</span>
oMyXScaling.Tick.Distance = <span class="HlNumbers">1</span>
oMyXScaling.MiniTickCount = <span class="HlNumbers">10</span>
<span class="HlVBSKeyword">Set</span> oMyYScaling = oMy2DAxisSystem.YAxis.Scaling
oMyYScaling.AutoScalingType = <span class="Hldiademconstant">eAxisAutoScalingManual</span>
oMyYScaling.Type = <span class="Hldiademconstant">e2DYScalingLinear</span>
oMyYScaling.Begin = <span class="HlNumbers">0</span>
oMyYScaling.End = <span class="HlNumbers">100</span>
oMyYScaling.Origin = <span class="HlNumbers">50</span>
oMyYScaling.Tick.Distance = <span class="HlNumbers">12</span>.<span class="HlNumbers">5</span>
oMyYScaling.MiniTickCount = <span class="HlNumbers">10</span>
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.Refresh</span>()</donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>dd.Report.NewLayout() 
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, <span class="HlString">"My2DAxisSystem"</span>) 
oMyPos = oMy2DAxisSystem.Position.ByCoordinate 
oMyPos.X1 = <span class="HlNumbers">20</span> 
oMyPos.X2 = <span class="HlNumbers">80</span> 
oMyPos.Y1 = <span class="HlNumbers">20</span> 
oMyPos.Y2 = <span class="HlNumbers">80</span> 
oMyXScaling = oMy2DAxisSystem.XAxis.Scaling 
oMyXScaling.AutoScalingType = dd.eAxisAutoScalingManual 
oMyXScaling.Type = dd.e2DXScalingLogarithmic 
oMyXScaling.Begin = <span class="HlNumbers">0</span>.<span class="HlNumbers">01</span> 
oMyXScaling.End = <span class="HlNumbers">100</span> 
oMyXScaling.Origin = <span class="HlNumbers">1</span> 
oMyXScaling.Tick.Distance = <span class="HlNumbers">1</span> 
oMyXScaling.MiniTickCount = <span class="HlNumbers">10</span> 
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling 
oMyYScaling.AutoScalingType = dd.eAxisAutoScalingManual 
oMyYScaling.Type = dd.e2DYScalingLinear 
oMyYScaling.Begin = <span class="HlNumbers">0</span> 
oMyYScaling.End = <span class="HlNumbers">100</span> 
oMyYScaling.Origin = <span class="HlNumbers">50</span> 
oMyYScaling.Tick.Distance = <span class="HlNumbers">12</span>.<span class="HlNumbers">5</span> 
oMyYScaling.MiniTickCount = <span class="HlNumbers">10</span> 
dd.Report.Refresh() 
		 </donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Origin_IRepD2AxisXScalingInt.htm`*
