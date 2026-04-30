---
title: "ITo2DConstantInt"
description: "The Constant object provides a constant in a 2D axis system in DIAdem VIEW. Use this object to specify the properties of the constants."
---

# ITo2DConstantInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Constant

The Constant object provides a constant in a 2D axis system in DIAdem VIEW. Use this object to specify the properties of the constants.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm")
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyChart = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyCurve = oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
oMyConstX = oMyChart.Constants.Add("30",0)
oMyConstX.Color = "red"
oMyConstY = oMyChart.Constants.Add("20",1)
oMyConstY.Color = "green"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ito2dconstantint-color/">Color</a> | <a href="../../properties/ito2dconstantint-colorrgb/">ColorRGB</a> | <a href="../../properties/ito2dconstantint-direction/">Direction</a> | <a href="../../properties/ito2dconstantint-index/">Index</a> | <a href="../../properties/ito2dconstantint-name/">Name</a> | <a href="../../properties/ito2dconstantint-valueexpression/">ValueExpression</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/constants/">Constants</a>.<a href="../../methods/ito2dconstantenumint-add/">Add</a> | <a href="../../collections/constants/">Constants</a>.<a href="../../methods/ito2dconstantenumint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_ITo2DConstantInt.htm`*
