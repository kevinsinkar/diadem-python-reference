---
title: "IToShaftCenterlineChartInt"
description: "The ShaftCenterline object provides access to a Shaft centerline axis system in DIAdem VIEW. Use the ShaftCenterline object to specify the properties of the axi"
---

# IToShaftCenterlineChartInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: ShaftCenterline

The ShaftCenterline object provides access to a Shaft centerline axis system in DIAdem VIEW. Use the ShaftCenterline object to specify the properties of the axis system.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\dd.Sound + Vibration\\RotatingShaftAnalysis_001.TDM")
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "ShaftCenterline"
oMyObj = oMySheet.ActiveArea.DisplayObj
oMyObj.CurvesShaftCenterline.Add("[1]/[2]","[1]/[3]")
oMyObj.AxisLabeling = True
oMyObj.DateTimePreference = eDateTimePreferenceAbsolute
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itoshaftcenterlinechartint-abscissa/">Abscissa</a> | <a href="../../properties/itoshaftcenterlinechartint-area/">Area</a> | <a href="../../properties/itoshaftcenterlinechartint-axislabeling/">AxisLabeling</a> | <a href="../../properties/itoshaftcenterlinechartint-bearingclearancehorizontal/">BearingClearanceHorizontal</a> | <a href="../../properties/itoshaftcenterlinechartint-bearingclearancevertical/">BearingClearanceVertical</a> | <a href="../../properties/itoshaftcenterlinechartint-curvesshaftcenterline/">CurvesShaftCenterline</a> | <a href="../../properties/itoshaftcenterlinechartint-datetimerepresentation/">DateTimeRepresentation</a> | <a href="../../properties/itoshaftcenterlinechartint-decorations/">Decorations</a> | <a href="../../properties/itoshaftcenterlinechartint-doublebuffered/">DoubleBuffered</a> | <a href="../../properties/itoshaftcenterlinechartint-lastzoommode/">LastZoomMode</a> | <a href="../../properties/itoshaftcenterlinechartint-legenditems/">LegendItems</a> | <a href="../../properties/itoshaftcenterlinechartint-legendwidth/">LegendWidth</a> | <a href="../../properties/itoshaftcenterlinechartint-ordinate/">Ordinate</a> | <a href="../../properties/itoshaftcenterlinechartint-rotationdirection/">RotationDirection</a> | <a href="../../properties/itoshaftcenterlinechartint-shaftrestingposition/">ShaftRestingPosition</a> | <a href="../../properties/itoshaftcenterlinechartint-toolbarvisible/">ToolbarVisible</a> | <a href="../../properties/itoshaftcenterlinechartint-xaxismargin/">XAxisMargin</a> | <a href="../../properties/itoshaftcenterlinechartint-xaxismarginmode/">XAxisMarginMode</a> | <a href="../../properties/itoshaftcenterlinechartint-xbegin/">XBegin</a> | <a href="../../properties/itoshaftcenterlinechartint-xend/">XEnd</a> | <a href="../../properties/itoshaftcenterlinechartint-xscalingmode/">XScalingMode</a> | <a href="../../properties/itoshaftcenterlinechartint-xsensorposition/">XSensorPosition</a> | <a href="../../properties/itoshaftcenterlinechartint-yaxismargin/">YAxisMargin</a> | <a href="../../properties/itoshaftcenterlinechartint-yaxismarginmode/">YAxisMarginMode</a> | <a href="../../properties/itoshaftcenterlinechartint-ybegin/">YBegin</a> | <a href="../../properties/itoshaftcenterlinechartint-yend/">YEnd</a> | <a href="../../properties/itoshaftcenterlinechartint-ysensorposition/">YSensorPosition</a> | <a href="../../properties/itoshaftcenterlinechartint-zoomcursor/">ZoomCursor</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itoshaftcenterlinechartint-showcurvesdlg/">ShowCurvesDlg</a> | <a href="../../methods/itoshaftcenterlinechartint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
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

*Source: `Scriptview/objects/VIEW_Objects_IToShaftCenterlineChartInt.htm`*
