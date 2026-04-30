---
title: "OrbitCurves"
description: "The OrbitCurves object provides a collection of all Curves in an orbit axis system in DIAdem VIEW. Use the OrbitCurves collection to delete curves or to add new"
---

# OrbitCurves

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: OrbitCurves

The OrbitCurves object provides a collection of all Curves in an orbit axis system in DIAdem VIEW. Use the OrbitCurves collection to delete curves or to add new curves.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\dd.Sound + Vibration\\RotatingShaftAnalysis_001.TDM")
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Orbit"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyChart.CurvesOrbit.Add("[1]/[1]","[1]/[2]")
oMyDecoPicture = oMyChart.Decorations.Add(dd.eVIEWDecorationTypePicture,"DecoPicture")
oMyDecoPicture.FileName = dd.ProgramDrv + "Examples/Documents/Example1.gif"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itoorbitcurveenumint-count/">Count</a> | <a href="../../properties/itoorbitcurveenumint-currcurve/">CurrCurve</a> | <a href="../../properties/itoorbitcurveenumint-leadingcurve/">LeadingCurve</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itoorbitcurveenumint-add/">Add</a> | <a href="../../methods/itoorbitcurveenumint-copy/">Copy</a> | <a href="../../methods/itoorbitcurveenumint-item/">Item</a> | <a href="../../methods/itoorbitcurveenumint-remove/">Remove</a> | <a href="../../methods/itoorbitcurveenumint-removeall/">RemoveAll</a> | <a href="../../methods/itoorbitcurveenumint-setleadingcurve/">SetLeadingCurve</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itoorbitchartint/">Orbit</a>.<a href="../../properties/itoorbitchartint-curvesorbit/">CurvesOrbit</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToOrbitCurveEnumInt.htm`*
