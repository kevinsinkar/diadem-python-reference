---
title: "ITo2DConstantInt.ColorRGB"
description: "Specifies the color of a constant in a 2D axis system in DIAdem VIEW. DIAdem only includes the color when the Color property has the value other colors ."
---

# ITo2DConstantInt.ColorRGB

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: ColorRGB for Constant

Specifies the color of a constant in a 2D axis system in DIAdem VIEW. DIAdem only includes the color when the Color property has the value other colors .

## Signature

```python
obj.ColorRGB
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyDisplayObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyDisplayObj.Curves2D.Add("[1]/[1]","[1]/[2]")
oMyDisplayObj.Constants.Add("5",0)
oMyDisplayObj.Constants(1).Name ="X constant"
oMyDisplayObj.Constants(1).Direction =1
oMyDisplayObj.Constants(1).Color ="other colors"
oMyDisplayObj.Constants(1).ColorRGB = dd.RGB(0,0,221)
oMyDisplayObj.Constants(1).ValueExpression =20
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_ColorRGB_ITo2DConstantInt.htm`*
