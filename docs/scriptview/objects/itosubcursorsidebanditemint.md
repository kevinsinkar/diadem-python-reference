---
title: "IToSubCursorSidebandItemInt"
description: "The Sideband object provides a cursor line of a Sideband cursor in a 2D axis system in DIAdem VIEW."
---

# IToSubCursorSidebandItemInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Sideband

The Sideband object provides a cursor line of a Sideband cursor in a 2D axis system in DIAdem VIEW.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyChart = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyCurve = oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
oMyObj = oMySheet.ActiveArea
oMyObj.DisplayObj.SubCursorType = dd.eVIEWSubCursorTypeSideband
oMySubCursor = oMySheet.ActiveArea.DisplayObj.SubCursor.Sidebands
sOutput = "Position of Additional Cursor Lines: " + "\r\n"
for i in range( 1, oMySubCursor.Count+1):
    sOutput = sOutput + "Line " + i + " left:  " + "\t" + " X: " + oMySubCursor(i).XLeft + " Y: " + oMySubCursor(i).YLeft + "\r\n"
    sOutput = sOutput + "Line " + i + " right: " + "\t" + " X: " + oMySubCursor(i).XRight + " Y: " + oMySubCursor(i).YRight + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itosubcursorsidebanditemint-xleft/">XLeft</a> | <a href="../../properties/itosubcursorsidebanditemint-xright/">XRight</a> | <a href="../../properties/itosubcursorsidebanditemint-yleft/">YLeft</a> | <a href="../../properties/itosubcursorsidebanditemint-yright/">YRight</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/sidebands/">Sidebands</a>.<a href="../../methods/itosubcursorsidebandenumint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToSubCursorSidebandItemInt.htm`*
