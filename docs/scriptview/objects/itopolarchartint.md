---
title: "IToPolarChartInt"
description: "The Polar object provides access to a Polar axis system in DIAdem VIEW. Use the Polar object to display curves and to define curve legends."
---

# IToPolarChartInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Polar

The Polar object provides access to a Polar axis system in DIAdem VIEW. Use the Polar object to display curves and to define curve legends.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm")
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Polar"
oMyPolarObj = oMySheet.ActiveArea.DisplayObj
oMyPolarObj.CurvesPolar.Add("[5]/[1]","[5]/[2]")
oMyPolarObj.AxisLabeling = True
oMyPolarObj.DoubleBuffered = True
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itopolarchartint-area/">Area</a> | <a href="../../properties/itopolarchartint-axislabeling/">AxisLabeling</a> | <a href="../../properties/itopolarchartint-cursorsynchronisationangle/">CursorSynchronisationAngle</a> | <a href="../../properties/itopolarchartint-cursorsynchronisationradius/">CursorSynchronisationRadius</a> | <a href="../../properties/itopolarchartint-curvespolar/">CurvesPolar</a> | <a href="../../properties/itopolarchartint-datetimerepresentation/">DateTimeRepresentation</a> | <a href="../../properties/itopolarchartint-decorations/">Decorations</a> | <a href="../../properties/itopolarchartint-doublebuffered/">DoubleBuffered</a> | <a href="../../properties/itopolarchartint-legenditems/">LegendItems</a> | <a href="../../properties/itopolarchartint-legendwidth/">LegendWidth</a> | <a href="../../properties/itopolarchartint-radialscalingbegin/">RadialScalingBegin</a> | <a href="../../properties/itopolarchartint-radialscalingend/">RadialScalingEnd</a> | <a href="../../properties/itopolarchartint-radialscalingmode/">RadialScalingMode</a> | <a href="../../properties/itopolarchartint-scalingangledirection/">ScalingAngleDirection</a> | <a href="../../properties/itopolarchartint-scalingzeroangle/">ScalingZeroAngle</a> | <a href="../../properties/itopolarchartint-toolbarvisible/">ToolbarVisible</a> | <a href="../../properties/itopolarchartint-xbegin/">XBegin</a> | <a href="../../properties/itopolarchartint-xend/">XEnd</a> | <a href="../../properties/itopolarchartint-ybegin/">YBegin</a> | <a href="../../properties/itopolarchartint-yend/">YEnd</a> | <a href="../../properties/itopolarchartint-zoomcursor/">ZoomCursor</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itopolarchartint-iszoomed/">IsZoomed</a> | <a href="../../methods/itopolarchartint-showcurvesdlg/">ShowCurvesDlg</a> | <a href="../../methods/itopolarchartint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
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

*Source: `Scriptview/objects/VIEW_Objects_IToPolarChartInt.htm`*
