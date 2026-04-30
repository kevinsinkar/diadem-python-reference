---
title: "IToBirdsEyeViewBoundaryInt"
description: "The BirdsEyeViewBoundary object provides access to lane markings in a bird's eye view display in DIAdem VIEW."
---

# IToBirdsEyeViewBoundaryInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: BirdsEyeViewBoundary

The BirdsEyeViewBoundary object provides access to lane markings in a bird's eye view display in DIAdem VIEW.

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewBirdsEyeView")
oMySheet.ActiveArea.DisplayObjType = "BirdsEyeView"
oMyObjects = dd.View.ActiveSheet.ActiveArea.DisplayObj.BirdsEyeViewObjects
oMyObject = oMyObjects.AddBoundary("[1]/[1]","[1]/[2]","[1]/[3]","[1]/[4]","[1]/[5]","[1]/[6]")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itobirdseyeviewboundaryint-anglechannelname/">AngleChannelName</a> | <a href="../../properties/itobirdseyeviewboundaryint-clothoidchannelname/">ClothoidChannelName</a> | <a href="../../properties/itobirdseyeviewboundaryint-color/">Color</a> | <a href="../../properties/itobirdseyeviewboundaryint-colorrgb/">ColorRGB</a> | <a href="../../properties/itobirdseyeviewboundaryint-curvaturechannelname/">CurvatureChannelName</a> | <a href="../../properties/itobirdseyeviewboundaryint-enable/">Enable</a> | <a href="../../properties/itobirdseyeviewboundaryint-index/">Index</a> | <a href="../../properties/itobirdseyeviewboundaryint-lateraldistancechannelname/">LateralDistanceChannelName</a> | <a href="../../properties/itobirdseyeviewboundaryint-lengthchannelname/">LengthChannelName</a> | <a href="../../properties/itobirdseyeviewboundaryint-name/">Name</a> | <a href="../../properties/itobirdseyeviewboundaryint-synchronisationchannelname/">SynchronisationChannelName</a> | <a href="../../properties/itobirdseyeviewboundaryint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/birdseyeviewobjects/">BirdsEyeViewObjects</a>.<a href="../../methods/itobirdseyeviewobjectenumint-addboundary/">AddBoundary</a> | <a href="../../collections/birdseyeviewobjects/">BirdsEyeViewObjects</a>.<a href="../../methods/itobirdseyeviewobjectenumint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToBirdsEyeViewBoundaryInt.htm`*
