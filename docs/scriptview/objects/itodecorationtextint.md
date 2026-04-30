---
title: "IToDecorationTextInt"
description: "The DecorationText object provides a Text type decoration in an axis system in DIAdem VIEW. Use the DecorationText object to specify the text properties. Decora"
---

# IToDecorationTextInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: DecorationText

The DecorationText object provides a Text type decoration in an axis system in DIAdem VIEW. Use the DecorationText object to specify the text properties. Decorations, such as texts or graphics can be used in 2D Axis Systems , Polar Axis Systems , Orbit Axis Systems , and Shaft Centerline Axis Systems .

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.Name = "MySheet"
oMySheet.ActiveArea.DisplayObjType = "Orbit"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyDecoText = oMyChart.Decorations.Add(dd.eVIEWDecorationTypeText,"DecoText")
oMyDecoText.Text = "Text as Decoration"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itodecorationtextint-index/">Index</a> | <a href="../../properties/itodecorationtextint-name/">Name</a> | <a href="../../properties/itodecorationtextint-positionhorizontal/">PositionHorizontal</a> | <a href="../../properties/itodecorationtextint-positionvertical/">PositionVertical</a> | <a href="../../properties/itodecorationtextint-text/">Text</a> | <a href="../../properties/itodecorationtextint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/decorations/">Decorations</a>.<a href="../../methods/itodecorationlistint-add/">Add</a> | <a href="../../collections/decorations/">Decorations</a>.<a href="../../methods/itodecorationlistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToDecorationTextInt.htm`*
