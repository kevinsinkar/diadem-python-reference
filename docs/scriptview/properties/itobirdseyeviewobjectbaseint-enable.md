---
title: "IToBirdsEyeViewObjectBaseInt.Enable"
description: "Specifies whether DIAdem VIEW displays an object in a bird's eye view display. The object can be a BirdsEyeViewBoundary object or a BirdsEyeViewDynamicObject ob"
---

# IToBirdsEyeViewObjectBaseInt.Enable

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Enable for BirdsEyeViewObjectBase

Specifies whether DIAdem VIEW displays an object in a bird's eye view display. The object can be a BirdsEyeViewBoundary object or a BirdsEyeViewDynamicObject objekt .

## Signature

```python
obj.Enable
```

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewBirdsEyeView")
oMySheet.ActiveArea.DisplayObjType = "BirdsEyeView"
oMyObjects = dd.View.ActiveSheet.ActiveArea.DisplayObj.BirdsEyeViewObjects
oMyObject1 = oMyObjects.AddBoundary("[1]/[1]","[1]/[2]","[1]/[3]","[1]/[4]","[1]/[5]","[1]/[6]")
oMyObject2 = oMyObjects.AddBoundary("[2]/[1]","[2]/[2]","[2]/[3]","[2]/[4]","[2]/[5]","[2]/[6]")
oMyObject1.Enable = False
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Enable_IToBirdsEyeViewObjectBaseInt.htm`*
