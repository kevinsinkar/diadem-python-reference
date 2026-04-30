---
title: "IToOrbitCurveInt"
description: "The OrbitCurve object provides access to a curve in an orbit axis system in DIAdem VIEW. Use the OrbitCurve object to specify the curve properties."
---

# IToOrbitCurveInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: OrbitCurve

The OrbitCurve object provides access to a curve in an orbit axis system in DIAdem VIEW. Use the OrbitCurve object to specify the curve properties.

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
<p><a href="../../properties/itoorbitcurveint-color/">Color</a> | <a href="../../properties/itoorbitcurveint-colorrgb/">ColorRGB</a> | <a href="../../properties/itoorbitcurveint-enable/">Enable</a> | <a href="../../properties/itoorbitcurveint-index/">Index</a> | <a href="../../properties/itoorbitcurveint-isvalid/">IsValid</a> | <a href="../../properties/itoorbitcurveint-labelatbegin/">LabelAtBegin</a> | <a href="../../properties/itoorbitcurveint-labelatend/">LabelAtEnd</a> | <a href="../../properties/itoorbitcurveint-labelchannelname/">LabelChannelName</a> | <a href="../../properties/itoorbitcurveint-labelchannelorientation/">LabelChannelOrientation</a> | <a href="../../properties/itoorbitcurveint-labelcolor/">LabelColor</a> | <a href="../../properties/itoorbitcurveint-labelcolorauto/">LabelColorAuto</a> | <a href="../../properties/itoorbitcurveint-labelcolorrgb/">LabelColorRGB</a> | <a href="../../properties/itoorbitcurveint-labelindexchannelname/">LabelIndexChannelName</a> | <a href="../../properties/itoorbitcurveint-labelintervallength/">LabelIntervalLength</a> | <a href="../../properties/itoorbitcurveint-labelintervalpoints/">LabelIntervalPoints</a> | <a href="../../properties/itoorbitcurveint-labelmode/">LabelMode</a> | <a href="../../properties/itoorbitcurveint-labelrepetitionmode/">LabelRepetitionMode</a> | <a href="../../properties/itoorbitcurveint-labeltext/">LabelText</a> | <a href="../../properties/itoorbitcurveint-markeratbegin/">MarkerAtBegin</a> | <a href="../../properties/itoorbitcurveint-markeratend/">MarkerAtEnd</a> | <a href="../../properties/itoorbitcurveint-markercolor/">MarkerColor</a> | <a href="../../properties/itoorbitcurveint-markercolorauto/">MarkerColorAuto</a> | <a href="../../properties/itoorbitcurveint-markercolorrgb/">MarkerColorRGB</a> | <a href="../../properties/itoorbitcurveint-markerfillcolor/">MarkerFillColor</a> | <a href="../../properties/itoorbitcurveint-markerfillcolorauto/">MarkerFillColorAuto</a> | <a href="../../properties/itoorbitcurveint-markerfillcolorrgb/">MarkerFillColorRGB</a> | <a href="../../properties/itoorbitcurveint-markerfrequencymode/">MarkerFrequencyMode</a> | <a href="../../properties/itoorbitcurveint-markerintervallength/">MarkerIntervalLength</a> | <a href="../../properties/itoorbitcurveint-markerintervalpoints/">MarkerIntervalPoints</a> | <a href="../../properties/itoorbitcurveint-markerlinewidth/">MarkerLineWidth</a> | <a href="../../properties/itoorbitcurveint-markersize/">MarkerSize</a> | <a href="../../properties/itoorbitcurveint-markertype/">MarkerType</a> | <a href="../../properties/itoorbitcurveint-name/">Name</a> | <a href="../../properties/itoorbitcurveint-selected/">Selected</a> | <a href="../../properties/itoorbitcurveint-tagstored/">TagStored</a> | <a href="../../properties/itoorbitcurveint-tagtemporary/">TagTemporary</a> | <a href="../../properties/itoorbitcurveint-type/">Type</a> | <a href="../../properties/itoorbitcurveint-visibleinlegend/">VisibleInLegend</a> | <a href="../../properties/itoorbitcurveint-xchannelname/">XChannelName</a> | <a href="../../properties/itoorbitcurveint-ychannelname/">YChannelName</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/orbitcurves/">OrbitCurves</a>.<a href="../../methods/itoorbitcurveenumint-add/">Add</a> | <a href="../../collections/orbitcurves/">OrbitCurves</a>.<a href="../../methods/itoorbitcurveenumint-copy/">Copy</a> | <a href="../../collections/orbitcurves/">OrbitCurves</a>.<a href="../../properties/itoorbitcurveenumint-currcurve/">CurrCurve</a> | <a href="../../collections/orbitcurves/">OrbitCurves</a>.<a href="../../methods/itoorbitcurveenumint-item/">Item</a> | <a href="../../collections/orbitcurves/">OrbitCurves</a>.<a href="../../properties/itoorbitcurveenumint-leadingcurve/">LeadingCurve</a> | <a href="../../collections/orbitcurves/">OrbitCurves</a>.<a href="../../methods/itoorbitcurveenumint-setleadingcurve/">SetLeadingCurve</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToOrbitCurveInt.htm`*
