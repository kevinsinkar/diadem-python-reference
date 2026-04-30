---
title: "ITo2DCurveInt"
description: "The 2DCurve object provides a curve in a 2D axis system in DIAdem VIEW. Use the Curve object to specify the curve properties."
---

# ITo2DCurveInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: 2DCurve

The 2DCurve object provides a curve in a 2D axis system in DIAdem VIEW. Use the Curve object to specify the curve properties.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm")
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyChart = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyCurve = oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ito2dcurveint-color/">Color</a> | <a href="../../properties/ito2dcurveint-colorrgb/">ColorRGB</a> | <a href="../../properties/ito2dcurveint-curverelatedyscalingname/">CurveRelatedYScalingName</a> | <a href="../../properties/ito2dcurveint-enable/">Enable</a> | <a href="../../properties/ito2dcurveint-index/">Index</a> | <a href="../../properties/ito2dcurveint-isvalid/">IsValid</a> | <a href="../../properties/ito2dcurveint-labelatbegin/">LabelAtBegin</a> | <a href="../../properties/ito2dcurveint-labelatend/">LabelAtEnd</a> | <a href="../../properties/ito2dcurveint-labelchannelname/">LabelChannelName</a> | <a href="../../properties/ito2dcurveint-labelchannelorientation/">LabelChannelOrientation</a> | <a href="../../properties/ito2dcurveint-labelcolor/">LabelColor</a> | <a href="../../properties/ito2dcurveint-labelcolorauto/">LabelColorAuto</a> | <a href="../../properties/ito2dcurveint-labelcolorrgb/">LabelColorRGB</a> | <a href="../../properties/ito2dcurveint-labelindexchannelname/">LabelIndexChannelName</a> | <a href="../../properties/ito2dcurveint-labelintervallength/">LabelIntervalLength</a> | <a href="../../properties/ito2dcurveint-labelintervalpoints/">LabelIntervalPoints</a> | <a href="../../properties/ito2dcurveint-labelmode/">LabelMode</a> | <a href="../../properties/ito2dcurveint-labelrepetitionmode/">LabelRepetitionMode</a> | <a href="../../properties/ito2dcurveint-labeltext/">LabelText</a> | <a href="../../properties/ito2dcurveint-markeratbegin/">MarkerAtBegin</a> | <a href="../../properties/ito2dcurveint-markeratend/">MarkerAtEnd</a> | <a href="../../properties/ito2dcurveint-markercolor/">MarkerColor</a> | <a href="../../properties/ito2dcurveint-markercolorauto/">MarkerColorAuto</a> | <a href="../../properties/ito2dcurveint-markercolorrgb/">MarkerColorRGB</a> | <a href="../../properties/ito2dcurveint-markerfillcolor/">MarkerFillColor</a> | <a href="../../properties/ito2dcurveint-markerfillcolorauto/">MarkerFillColorAuto</a> | <a href="../../properties/ito2dcurveint-markerfillcolorrgb/">MarkerFillColorRGB</a> | <a href="../../properties/ito2dcurveint-markerfrequencymode/">MarkerFrequencyMode</a> | <a href="../../properties/ito2dcurveint-markerintervallength/">MarkerIntervalLength</a> | <a href="../../properties/ito2dcurveint-markerintervalpoints/">MarkerIntervalPoints</a> | <a href="../../properties/ito2dcurveint-markerlinewidth/">MarkerLineWidth</a> | <a href="../../properties/ito2dcurveint-markersize/">MarkerSize</a> | <a href="../../properties/ito2dcurveint-markertype/">MarkerType</a> | <a href="../../properties/ito2dcurveint-name/">Name</a> | <a href="../../properties/ito2dcurveint-selected/">Selected</a> | <a href="../../properties/ito2dcurveint-tagstored/">TagStored</a> | <a href="../../properties/ito2dcurveint-tagtemporary/">TagTemporary</a> | <a href="../../properties/ito2dcurveint-type/">Type</a> | <a href="../../properties/ito2dcurveint-visibleinlegend/">VisibleInLegend</a> | <a href="../../properties/ito2dcurveint-xchannelname/">XChannelName</a> | <a href="../../properties/ito2dcurveint-ychannelname/">YChannelName</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/2dcurves/">2DCurves</a>.<a href="../../methods/ito2dcurveenumint-add/">Add</a> | <a href="../../collections/2dcurves/">2DCurves</a>.<a href="../../methods/ito2dcurveenumint-copy/">Copy</a> | <a href="../../collections/2dcurves/">2DCurves</a>.<a href="../../properties/ito2dcurveenumint-currcurve/">CurrCurve</a> | <a href="../../collections/2dcurves/">2DCurves</a>.<a href="../../methods/ito2dcurveenumint-item/">Item</a> | <a href="../../collections/2dcurves/">2DCurves</a>.<a href="../../properties/ito2dcurveenumint-leadingcurve/">LeadingCurve</a> | <a href="../../collections/2dcurves/">2DCurves</a>.<a href="../../methods/ito2dcurveenumint-setleadingcurve/">SetLeadingCurve</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_ITo2DCurveInt.htm`*
