---
title: "IToBirdsEyeViewChartInt"
description: "The BirdsEyeView object provides a Bird's Eye View display in DIAdem VIEW. Use the BirdsEyeView object to specify the properties of the display."
---

# IToBirdsEyeViewChartInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: BirdsEyeView

The BirdsEyeView object provides a Bird's Eye View display in DIAdem VIEW. Use the BirdsEyeView object to specify the properties of the display.

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewBirdsEyeView")
oMySheet.ActiveArea.DisplayObjType = "BirdsEyeView"
oMyObjects = dd.View.ActiveSheet.ActiveArea.DisplayObj.BirdsEyeViewObjects
oMyObject = oMyObjects.AddDynamicObject("[1]/[1]","[1]/[2]","[1]/[3]")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itobirdseyeviewchartint-area/">Area</a> | <a href="../../properties/itobirdseyeviewchartint-axislabeling/">AxisLabeling</a> | <a href="../../properties/itobirdseyeviewchartint-birdseyeviewobjects/">BirdsEyeViewObjects</a> | <a href="../../properties/itobirdseyeviewchartint-deltax/">DeltaX</a> | <a href="../../properties/itobirdseyeviewchartint-doublebuffered/">DoubleBuffered</a> | <a href="../../properties/itobirdseyeviewchartint-fieldsofview/">FieldsOfView</a> | <a href="../../properties/itobirdseyeviewchartint-lastzoommode/">LastZoomMode</a> | <a href="../../properties/itobirdseyeviewchartint-lateraldimension/">LateralDimension</a> | <a href="../../properties/itobirdseyeviewchartint-legendwidth/">LegendWidth</a> | <a href="../../properties/itobirdseyeviewchartint-longitudinaldimension/">LongitudinalDimension</a> | <a href="../../properties/itobirdseyeviewchartint-staticobject/">StaticObject</a> | <a href="../../properties/itobirdseyeviewchartint-synchronisationdimension/">SynchronisationDimension</a> | <a href="../../properties/itobirdseyeviewchartint-toolbarvisible/">ToolbarVisible</a> | <a href="../../properties/itobirdseyeviewchartint-useisometricaxes/">UseIsometricAxes</a> | <a href="../../properties/itobirdseyeviewchartint-xbegin/">XBegin</a> | <a href="../../properties/itobirdseyeviewchartint-xend/">XEnd</a> | <a href="../../properties/itobirdseyeviewchartint-ybegin/">YBegin</a> | <a href="../../properties/itobirdseyeviewchartint-yend/">YEnd</a> | <a href="../../properties/itobirdseyeviewchartint-yscalingbegin/">YScalingBegin</a> | <a href="../../properties/itobirdseyeviewchartint-yscalingend/">YScalingEnd</a> | <a href="../../properties/itobirdseyeviewchartint-yscalingmode/">YScalingMode</a> | <a href="../../properties/itobirdseyeviewchartint-zoomcursor/">ZoomCursor</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itobirdseyeviewchartint-showcurvesdlg/">ShowCurvesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itoareaobjectint/">Area</a>.<a href="../../properties/itoareaobjectint-displayobj/">DisplayObj</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToBirdsEyeViewChartInt.htm`*
