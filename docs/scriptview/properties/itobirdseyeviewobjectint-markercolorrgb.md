---
title: "IToBirdsEyeViewObjectInt.MarkerColorRGB"
description: "Specifies the fill color of the markers of a dynamic object in a bird's eye view display in DIAdem VIEW. DIAdem only includes the color when the MarkerColor pro"
---

# IToBirdsEyeViewObjectInt.MarkerColorRGB

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: MarkerColorRGB for BirdsEyeViewDynamicObject

Specifies the fill color of the markers of a dynamic object in a bird's eye view display in DIAdem VIEW. DIAdem only includes the color when the MarkerColor property has the value other colors . Use a RGB value or a VBS color constant to specify the color.

## Signature

```python
obj.MarkerColorRGB
```

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewBirdsEyeView")
oMySheet.ActiveArea.DisplayObjType = "BirdsEyeView"
oMyObjects = dd.View.ActiveSheet.ActiveArea.DisplayObj.BirdsEyeViewObjects
oMyObject = oMyObjects.AddDynamicObject("[1]/[1]","[1]/[2]","[1]/[3]")
oMyObject.MarkerType = "square"
oMyObject.MarkerColor = "other colors"
oMyObject.MarkerColorRGB = dd.RGB(0,0,221)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_MarkerColorRGB_IToBirdsEyeViewObjectInt.htm`*
