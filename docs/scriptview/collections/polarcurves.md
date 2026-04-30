---
title: "PolarCurves"
description: "The PolarCurves object provides a collection of all Curves in a polar axis system in DIAdem VIEW. Use the PolarCurves collection to delete curves or to add new "
---

# PolarCurves

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: PolarCurves

The PolarCurves object provides a collection of all Curves in a polar axis system in DIAdem VIEW. Use the PolarCurves collection to delete curves or to add new curves.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm")
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Polar"
oMyPolarObj = oMySheet.ActiveArea.DisplayObj
oMyPolarObj.CurvesPolar.Add("[5]/[1]","[5]/[2]")
oMyPolarObj.AxisLabeling = True
oMyPolarObj.DoubleBuffered = True
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itopolarcurveenumint-count/">Count</a> | <a href="../../properties/itopolarcurveenumint-currcurve/">CurrCurve</a> | <a href="../../properties/itopolarcurveenumint-leadingcurve/">LeadingCurve</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itopolarcurveenumint-add/">Add</a> | <a href="../../methods/itopolarcurveenumint-copy/">Copy</a> | <a href="../../methods/itopolarcurveenumint-item/">Item</a> | <a href="../../methods/itopolarcurveenumint-remove/">Remove</a> | <a href="../../methods/itopolarcurveenumint-removeall/">RemoveAll</a> | <a href="../../methods/itopolarcurveenumint-setleadingcurve/">SetLeadingCurve</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itopolarchartint/">Polar</a>.<a href="../../properties/itopolarchartint-curvespolar/">CurvesPolar</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToPolarCurveEnumInt.htm`*
