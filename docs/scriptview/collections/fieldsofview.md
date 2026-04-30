---
title: "FieldsOfView"
description: "Collection of FieldOfView objects in the bird's eye view display in DIAdem VIEW."
---

# FieldsOfView

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: FieldsOfView

Collection of FieldOfView objects in the bird's eye view display in DIAdem VIEW.

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewBirdsEyeView")
oMySheet.ActiveArea.DisplayObjType = "BirdsEyeView"
oMyObjects = dd.View.ActiveSheet.ActiveArea.DisplayObj.FieldsOfView
oMyObject = oMyObjects.Add(0, 0, 0, 50, 50, 50)
dd.LogfileWrite("Lateral Distance: " + dd.Str(oMyObject.LateralDistance) + "\r\n" + "Longitudinal Distance: " + dd.Str(oMyObject.LongitudinalDistance) + "\r\n" + "Orientation Angle: " + dd.Str(oMyObject.OrientationAngle) + "\r\n" + "Aperture Angle: " + dd.Str(oMyObject.ApertureAngle) + "\r\n" + "Radius: " + dd.Str(oMyObject.Radius) + "\r\n" + "Fill Transparency: " + dd.Str(oMyObject.FillTransparency))
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itofieldofviewlistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itofieldofviewlistint-add/">Add</a> | <a href="../../methods/itofieldofviewlistint-exists/">Exists</a> | <a href="../../methods/itofieldofviewlistint-item/">Item</a> | <a href="../../methods/itofieldofviewlistint-remove/">Remove</a> | <a href="../../methods/itofieldofviewlistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itobirdseyeviewchartint/">BirdsEyeView</a>.<a href="../../properties/itobirdseyeviewchartint-fieldsofview/">FieldsOfView</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToFieldOfViewListInt.htm`*
