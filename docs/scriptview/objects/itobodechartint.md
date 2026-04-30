---
title: "IToBodeChartInt"
description: "The Bode object provides a Bode axis system in DIAdem VIEW. Use the Bode object to specify the properties of the axis system."
---

# IToBodeChartInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Bode

The Bode object provides a Bode axis system in DIAdem VIEW. Use the Bode object to specify the properties of the axis system.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.Name = "MySheet"
oMySheet.ActiveArea.DisplayObjType = "Bode"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyChart.CurvesBode.Add("[1]/[1]","[1]/[2]","[1]/[3]")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itobodechartint-activesystem/">ActiveSystem</a> | <a href="../../properties/itobodechartint-amplitudebegin/">AmplitudeBegin</a> | <a href="../../properties/itobodechartint-amplitudeend/">AmplitudeEnd</a> | <a href="../../properties/itobodechartint-amplitudescalingbegin/">AmplitudeScalingBegin</a> | <a href="../../properties/itobodechartint-amplitudescalingend/">AmplitudeScalingEnd</a> | <a href="../../properties/itobodechartint-amplitudescalingmode/">AmplitudeScalingMode</a> | <a href="../../properties/itobodechartint-amplitudescalingtype/">AmplitudeScalingType</a> | <a href="../../properties/itobodechartint-area/">Area</a> | <a href="../../properties/itobodechartint-axislabeling/">AxisLabeling</a> | <a href="../../properties/itobodechartint-chartdivisionratio/">ChartDivisionRatio</a> | <a href="../../properties/itobodechartint-cursorsynchronisationamplitude/">CursorSynchronisationAmplitude</a> | <a href="../../properties/itobodechartint-cursorsynchronisationphase/">CursorSynchronisationPhase</a> | <a href="../../properties/itobodechartint-cursorsynchronisationx/">CursorSynchronisationX</a> | <a href="../../properties/itobodechartint-curvesbode/">CurvesBode</a> | <a href="../../properties/itobodechartint-doublebuffered/">DoubleBuffered</a> | <a href="../../properties/itobodechartint-lastzoommode/">LastZoomMode</a> | <a href="../../properties/itobodechartint-legenditems/">LegendItems</a> | <a href="../../properties/itobodechartint-legendwidth/">LegendWidth</a> | <a href="../../properties/itobodechartint-marginbottom/">MarginBottom</a> | <a href="../../properties/itobodechartint-marginbottommode/">MarginBottomMode</a> | <a href="../../properties/itobodechartint-marginleft/">MarginLeft</a> | <a href="../../properties/itobodechartint-marginleftmode/">MarginLeftMode</a> | <a href="../../properties/itobodechartint-phasebegin/">PhaseBegin</a> | <a href="../../properties/itobodechartint-phaseend/">PhaseEnd</a> | <a href="../../properties/itobodechartint-phasescalingbegin/">PhaseScalingBegin</a> | <a href="../../properties/itobodechartint-phasescalingend/">PhaseScalingEnd</a> | <a href="../../properties/itobodechartint-phasescalingmode/">PhaseScalingMode</a> | <a href="../../properties/itobodechartint-toolbarvisible/">ToolbarVisible</a> | <a href="../../properties/itobodechartint-xbegin/">XBegin</a> | <a href="../../properties/itobodechartint-xend/">XEnd</a> | <a href="../../properties/itobodechartint-xscalingmode/">XScalingMode</a> | <a href="../../properties/itobodechartint-xscalingtype/">XScalingType</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itobodechartint-showcurvesdlg/">ShowCurvesDlg</a> | <a href="../../methods/itobodechartint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
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

*Source: `Scriptview/objects/VIEW_Objects_IToBodeChartInt.htm`*
