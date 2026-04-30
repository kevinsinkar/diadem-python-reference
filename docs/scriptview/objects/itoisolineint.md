---
title: "IToIsolineInt"
description: "The Isoline object provides access to an isoline of a contour display in DIAdem VIEW. Use the Isoline object to define the display of the isoline."
---

# IToIsolineInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Isoline

The Isoline object provides access to an isoline of a contour display in DIAdem VIEW. Use the Isoline object to define the display of the isoline.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples/Data/View_Contour.tdm")
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Contour"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyContour = oMyChart.CurvesContour.AddContour("[1]/[1]","[1]/[2]","[1]/[3]")
oMyContour.Structure = "Triplet"
oMyContour.ColoringType = "Gradient"
oMyIsoline = oMyChart.CurvesContour.AddIsoline("[1]/[1]","[1]/[2]")
oMyIsoline.Color = "black"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itoisolineint-color/">Color</a> | <a href="../../properties/itoisolineint-colorrgb/">ColorRGB</a> | <a href="../../properties/itoisolineint-displayisolinevalues/">DisplayIsolineValues</a> | <a href="../../properties/itoisolineint-index/">Index</a> | <a href="../../properties/itoisolineint-name/">Name</a> | <a href="../../properties/itoisolineint-tagstored/">TagStored</a> | <a href="../../properties/itoisolineint-tagtemporary/">TagTemporary</a> | <a href="../../properties/itoisolineint-type/">Type</a> | <a href="../../properties/itoisolineint-xchannelname/">XChannelName</a> | <a href="../../properties/itoisolineint-ychannelname/">YChannelName</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/contourcurves/">ContourCurves</a>.<a href="../../methods/itocontourcurveenumint-addisoline/">AddIsoline</a> | <a href="../../collections/contourcurves/">ContourCurves</a>.<a href="../../properties/itocontourcurveenumint-currcurve/">CurrCurve</a> | <a href="../../collections/contourcurves/">ContourCurves</a>.<a href="../../methods/itocontourcurveenumint-item/">Item</a> | <a href="../../collections/contourcurves/">ContourCurves</a>.<a href="../../properties/itocontourcurveenumint-leadingcurve/">LeadingCurve</a> | <a href="../../collections/contourcurves/">ContourCurves</a>.<a href="../../methods/itocontourcurveenumint-setleadingcurve/">SetLeadingCurve</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Creating a Python Graphic with a Pie Chart in VIEW</a> | <a href="#" data-unresolved="1">Creating Areas</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Generating and Formatting Text</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Moving or Copying Areas</a> | <a href="#" data-unresolved="1">Partitioning Worksheets</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToIsolineInt.htm`*
