---
title: "IToCurveRelatedYScalingListInt.Count"
description: "Returns the number of curve-related y-scaling of a 2D axis system in DIAdem VIEW."
---

# IToCurveRelatedYScalingListInt.Count

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Count for CurveRelatedYScalings

Returns the number of curve-related y-scaling of a 2D axis system in DIAdem VIEW.

## Signature

```python
obj.Count
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
dd.MsgBoxDisp (dd.View.ActiveSheet.ActiveArea.DisplayObj.YScalingList.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Count_IToCurveRelatedYScalingListInt.htm`*
