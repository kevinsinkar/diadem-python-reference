---
title: "IToSubCursorDefInt"
description: "The SubCursor object provides access to additional cursor lines for the Cursor in DIAdem VIEW. Use the SubCursor object to specify the properties of the cursor "
---

# IToSubCursorDefInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: SubCursor

The SubCursor object provides access to additional cursor lines for the Cursor in DIAdem VIEW. Use the SubCursor object to specify the properties of the cursor lines.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyCurve = oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
oMyObj = oMySheet.ActiveArea
oMyObj.DisplayObj.SubCursorType = dd.eVIEWSubCursorTypeSideband
dd.MsgBoxDisp("Additional Cursor Lines: " + oMyObj.DisplayObj.SubCursor.Sidebands.Count + "\r\n" + "Cursor Line Interval: " + oMyObj.DisplayObj.SubCursor.Sidebands.Interval)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itosubcursordefint-harmoniccount/">HarmonicCount</a> | <a href="../../properties/itosubcursordefint-sidebandcount/">SidebandCount</a> | <a href="../../properties/itosubcursordefint-sidebandinterval/">SidebandInterval</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itocursormasterint/">Cursor</a>.<a href="../../properties/itocursormasterint-subcursor/">SubCursor</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToSubCursorDefInt.htm`*
