---
title: "IToBirdsEyeViewBoundaryInt.CurvatureChannelName"
description: "Specifies the name of the channel that contains the curvature of the lane markings in a bird's eye view display in DIAdem VIEW."
---

# IToBirdsEyeViewBoundaryInt.CurvatureChannelName

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: CurvatureChannelName for BirdsEyeViewBoundary

Specifies the name of the channel that contains the curvature of the lane markings in a bird's eye view display in DIAdem VIEW.

## Signature

```python
obj.CurvatureChannelName
```

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewBirdsEyeView")
oMySheet.ActiveArea.DisplayObjType = "BirdsEyeView"
oMyObjects = dd.View.ActiveSheet.ActiveArea.DisplayObj.BirdsEyeViewObjects
oMyObject = oMyObjects.AddBoundary("[1]/[1]","[1]/[2]","[1]/[3]","[1]/[4]","[1]/[5]","[1]/[6]")
dd.LogfileWrite("Synchronisation channel: " + oMyObject.SynchronisationChannelName + "\r\n" + "Lateral distance: " + oMyObject.LateralDistanceChannelName + "\r\n" + "Angle: " + oMyObject.AngleChannelName + "\r\n"  + "Curvature: " + oMyObject.CurvatureChannelName + "\r\n" + "Clothoid: " + oMyObject.ClothoidChannelName + "\r\n" + "Length: " + oMyObject.LengthChannelName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_CurvatureChannelName_IToBirdsEyeViewBoundaryInt.htm`*
