---
title: "BodeCurves"
description: "The BodeCurves object provides a collection of all Curves in a Bode axis system in DIAdem VIEW. Use the BodeCurves collection to delete curves or to add new cur"
---

# BodeCurves

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: BodeCurves

The BodeCurves object provides a collection of all Curves in a Bode axis system in DIAdem VIEW. Use the BodeCurves collection to delete curves or to add new curves.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Bode"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyChart.CurvesBode.Add("[1]/[1]","[1]/[2]","[1]/[3]")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itobodecurveenumint-count/">Count</a> | <a href="../../properties/itobodecurveenumint-currcurve/">CurrCurve</a> | <a href="../../properties/itobodecurveenumint-leadingcurve/">LeadingCurve</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itobodecurveenumint-add/">Add</a> | <a href="../../methods/itobodecurveenumint-copy/">Copy</a> | <a href="../../methods/itobodecurveenumint-item/">Item</a> | <a href="../../methods/itobodecurveenumint-remove/">Remove</a> | <a href="../../methods/itobodecurveenumint-removeall/">RemoveAll</a> | <a href="../../methods/itobodecurveenumint-setleadingcurve/">SetLeadingCurve</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itobodechartint/">Bode</a>.<a href="../../properties/itobodechartint-curvesbode/">CurvesBode</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToBodeCurveEnumInt.htm`*
