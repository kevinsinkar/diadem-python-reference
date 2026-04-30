---
title: "Decorations"
description: "The Decoration object provides a collection of Texts and Graphics as layout elements for axis systems in DIAdem VIEW. Use the Decorations collection to delete d"
---

# Decorations

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: Decorations

The Decoration object provides a collection of Texts and Graphics as layout elements for axis systems in DIAdem VIEW. Use the Decorations collection to delete decorations or to add new decorations. Decorations are possible in 2D Axis Systems and also in Polar , Orbit , and Shaft Centerline axis systems .

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Orbit"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyChart.CurvesOrbit.Add("[1]/[1]","[1]/[2]")
oMyDecoText = oMyChart.Decorations.Add(dd.eVIEWDecorationTypeText,"DecoText")
oMyDecoText.Text = "Text as Decoration"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itodecorationlistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itodecorationlistint-add/">Add</a> | <a href="../../methods/itodecorationlistint-exists/">Exists</a> | <a href="../../methods/itodecorationlistint-item/">Item</a> | <a href="../../methods/itodecorationlistint-remove/">Remove</a> | <a href="../../methods/itodecorationlistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ito2dchartint/">CurveChart2D</a>.<a href="../../properties/ito2dchartint-decorations/">Decorations</a> | <a href="../../objects/itoorbitchartint/">Orbit</a>.<a href="../../properties/itoorbitchartint-decorations/">Decorations</a> | <a href="../../objects/itopolarchartint/">Polar</a>.<a href="../../properties/itopolarchartint-decorations/">Decorations</a> | <a href="../../objects/itoshaftcenterlinechartint/">ShaftCenterline</a>.<a href="../../properties/itoshaftcenterlinechartint-decorations/">Decorations</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToDecorationListInt.htm`*
