---
title: "IToOrbitChartInt"
description: "The Orbit object provides access to an Orbit axis system in DIAdem VIEW. Use the Orbit object to specify the properties of the axis system."
---

# IToOrbitChartInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Orbit

The Orbit object provides access to an Orbit axis system in DIAdem VIEW. Use the Orbit object to specify the properties of the axis system.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\dd.Sound + Vibration\\RotatingShaftAnalysis_001.TDM")
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Orbit"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyChart.CurvesOrbit.Add("[1]/[1]","[1]/[2]")
oMyDecoPicture = oMyChart.Decorations.Add(dd.eVIEWDecorationTypePicture,"DecoPicture")
oMyDecoPicture.FileName = dd.ProgramDrv + "Examples/Documents/Example1.gif"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itoorbitchartint-abscissa/">Abscissa</a> | <a href="../../properties/itoorbitchartint-area/">Area</a> | <a href="../../properties/itoorbitchartint-axislabeling/">AxisLabeling</a> | <a href="../../properties/itoorbitchartint-bearingclearancehorizontal/">BearingClearanceHorizontal</a> | <a href="../../properties/itoorbitchartint-bearingclearancevertical/">BearingClearanceVertical</a> | <a href="../../properties/itoorbitchartint-bearingreference/">BearingReference</a> | <a href="../../properties/itoorbitchartint-curvesorbit/">CurvesOrbit</a> | <a href="../../properties/itoorbitchartint-datetimerepresentation/">DateTimeRepresentation</a> | <a href="../../properties/itoorbitchartint-decorations/">Decorations</a> | <a href="../../properties/itoorbitchartint-doublebuffered/">DoubleBuffered</a> | <a href="../../properties/itoorbitchartint-lastzoommode/">LastZoomMode</a> | <a href="../../properties/itoorbitchartint-legenditems/">LegendItems</a> | <a href="../../properties/itoorbitchartint-legendwidth/">LegendWidth</a> | <a href="../../properties/itoorbitchartint-ordinate/">Ordinate</a> | <a href="../../properties/itoorbitchartint-rotationdirection/">RotationDirection</a> | <a href="../../properties/itoorbitchartint-shaftrestingposition/">ShaftRestingPosition</a> | <a href="../../properties/itoorbitchartint-toolbarvisible/">ToolbarVisible</a> | <a href="../../properties/itoorbitchartint-xaxismargin/">XAxisMargin</a> | <a href="../../properties/itoorbitchartint-xaxismarginmode/">XAxisMarginMode</a> | <a href="../../properties/itoorbitchartint-xbegin/">XBegin</a> | <a href="../../properties/itoorbitchartint-xend/">XEnd</a> | <a href="../../properties/itoorbitchartint-xscalingmode/">XScalingMode</a> | <a href="../../properties/itoorbitchartint-xsensorposition/">XSensorPosition</a> | <a href="../../properties/itoorbitchartint-yaxismargin/">YAxisMargin</a> | <a href="../../properties/itoorbitchartint-yaxismarginmode/">YAxisMarginMode</a> | <a href="../../properties/itoorbitchartint-ybegin/">YBegin</a> | <a href="../../properties/itoorbitchartint-yend/">YEnd</a> | <a href="../../properties/itoorbitchartint-ysensorposition/">YSensorPosition</a> | <a href="../../properties/itoorbitchartint-zoomcursor/">ZoomCursor</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itoorbitchartint-showcurvesdlg/">ShowCurvesDlg</a> | <a href="../../methods/itoorbitchartint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
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

*Source: `Scriptview/objects/VIEW_Objects_IToOrbitChartInt.htm`*
