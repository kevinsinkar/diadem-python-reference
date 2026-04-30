---
title: "Harmonics"
description: "The Harmonics object provides a collection of additional cursor lines of an Harmonic cursor in a 2D Axis System system in DIAdem VIEW. The harmonics collection "
---

# Harmonics

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: Harmonics

The Harmonics object provides a collection of additional cursor lines of an Harmonic cursor in a 2D Axis System system in DIAdem VIEW. The harmonics collection provides the coordinates and the one-sided number of additional cursor lines.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyChart = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyCurve = oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
oMyObj = oMySheet.ActiveArea
oMyObj.DisplayObj.SubCursorType = dd.eVIEWSubCursorTypeHarmonic
oMySubCursor = oMySheet.ActiveArea.DisplayObj.SubCursor.Harmonics
dd.MsgBoxDisp("Additional Cursor Lines: " + oMySubCursor.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itosubcursorharmonicenumint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itosubcursorharmonicenumint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itosubcursorharmonicint/">HarmonicCursor</a>.<a href="../../properties/itosubcursorharmonicint-harmonics/">Harmonics</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToSubCursorHarmonicEnumInt.htm`*
