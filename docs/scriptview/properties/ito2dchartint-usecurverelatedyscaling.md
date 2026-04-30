---
title: "ITo2DChartInt.UseCurveRelatedYScaling"
description: "Enables the curve-related y-scaling in a 2D axis system in DIAdem VIEW."
---

# ITo2DChartInt.UseCurveRelatedYScaling

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: UseCurveRelatedYScaling for CurveChart2D

Enables the curve-related y-scaling in a 2D axis system in DIAdem VIEW.

## Signature

```python
obj.UseCurveRelatedYScaling
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>You can only apply curve-related y-scalings to a 2D axis system if <a href="../ito2dchartint-yscaling/">YScaling</a> is set to <span class="Monospace">n systems [phys.]</span> or <span class="Monospace">n axes [phys.]</span>.</td>
</tr>
</table>
</div>

## Python example

```python
dd.View.NewLayout()
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyChart = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyChart.YScaling = "n systems [phys.]"
oMyChart.UseCurveRelatedYScaling = True

oMyYScalingList = dd.view.ActiveSheet.ActiveArea.DisplayObj.YScalingList

oMyYScaling1 = oMyYScalingList.Add ("MyScaling1","Scale1")
oMyYScaling1.Mode = dd.eVIEWYScalingModeAutomatic

oMyYScaling2 = oMyYScalingList.Add ("MyScaling2","Scale2")
oMyYScaling2.Mode = dd.eVIEWYScalingModeManual
oMyYScaling2.Begin = 4000
oMyYScaling2.End = 7500

oMyCurve1 = oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
oMyCurve1.CurveRelatedYScalingName = "MyScaling1"
oMyCurve2 = oMyChart.Curves2D.Add("[1]/[1]","[1]/[3]")
oMyCurve2.CurveRelatedYScalingName = "MyScaling2"
oMyCurve3 = oMyChart.Curves2D.Add("[1]/[1]","[1]/[4]")
oMyCurve3.CurveRelatedYScalingName = "MyScaling1"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_UseCurveRelatedYScaling_ITo2DChartInt.htm`*
