---
title: "IToPolarCurveInt"
description: "The PolarCurve object provides access to a curve in a polar axis system in DIAdem VIEW. Use the PolarCurve object to specify the curve properties."
---

# IToPolarCurveInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: PolarCurve

The PolarCurve object provides access to a curve in a polar axis system in DIAdem VIEW. Use the PolarCurve object to specify the curve properties.

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
<p><a href="../../properties/itopolarcurveint-anglechannelname/">AngleChannelName</a> | <a href="../../properties/itopolarcurveint-color/">Color</a> | <a href="../../properties/itopolarcurveint-colorrgb/">ColorRGB</a> | <a href="../../properties/itopolarcurveint-enable/">Enable</a> | <a href="../../properties/itopolarcurveint-index/">Index</a> | <a href="../../properties/itopolarcurveint-isvalid/">IsValid</a> | <a href="../../properties/itopolarcurveint-labelatbegin/">LabelAtBegin</a> | <a href="../../properties/itopolarcurveint-labelatend/">LabelAtEnd</a> | <a href="../../properties/itopolarcurveint-labelchannelname/">LabelChannelName</a> | <a href="../../properties/itopolarcurveint-labelchannelorientation/">LabelChannelOrientation</a> | <a href="../../properties/itopolarcurveint-labelcolor/">LabelColor</a> | <a href="../../properties/itopolarcurveint-labelcolorauto/">LabelColorAuto</a> | <a href="../../properties/itopolarcurveint-labelcolorrgb/">LabelColorRGB</a> | <a href="../../properties/itopolarcurveint-labelindexchannelname/">LabelIndexChannelName</a> | <a href="../../properties/itopolarcurveint-labelintervallength/">LabelIntervalLength</a> | <a href="../../properties/itopolarcurveint-labelintervalpoints/">LabelIntervalPoints</a> | <a href="../../properties/itopolarcurveint-labelmode/">LabelMode</a> | <a href="../../properties/itopolarcurveint-labelrepetitionmode/">LabelRepetitionMode</a> | <a href="../../properties/itopolarcurveint-labeltext/">LabelText</a> | <a href="../../properties/itopolarcurveint-markeratbegin/">MarkerAtBegin</a> | <a href="../../properties/itopolarcurveint-markeratend/">MarkerAtEnd</a> | <a href="../../properties/itopolarcurveint-markercolor/">MarkerColor</a> | <a href="../../properties/itopolarcurveint-markercolorauto/">MarkerColorAuto</a> | <a href="../../properties/itopolarcurveint-markercolorrgb/">MarkerColorRGB</a> | <a href="../../properties/itopolarcurveint-markerfillcolor/">MarkerFillColor</a> | <a href="../../properties/itopolarcurveint-markerfillcolorauto/">MarkerFillColorAuto</a> | <a href="../../properties/itopolarcurveint-markerfillcolorrgb/">MarkerFillColorRGB</a> | <a href="../../properties/itopolarcurveint-markerfrequencymode/">MarkerFrequencyMode</a> | <a href="../../properties/itopolarcurveint-markerintervallength/">MarkerIntervalLength</a> | <a href="../../properties/itopolarcurveint-markerintervalpoints/">MarkerIntervalPoints</a> | <a href="../../properties/itopolarcurveint-markerlinewidth/">MarkerLineWidth</a> | <a href="../../properties/itopolarcurveint-markersize/">MarkerSize</a> | <a href="../../properties/itopolarcurveint-markertype/">MarkerType</a> | <a href="../../properties/itopolarcurveint-name/">Name</a> | <a href="../../properties/itopolarcurveint-radiuschannelname/">RadiusChannelName</a> | <a href="../../properties/itopolarcurveint-selected/">Selected</a> | <a href="../../properties/itopolarcurveint-tagstored/">TagStored</a> | <a href="../../properties/itopolarcurveint-tagtemporary/">TagTemporary</a> | <a href="../../properties/itopolarcurveint-type/">Type</a> | <a href="../../properties/itopolarcurveint-visibleinlegend/">VisibleInLegend</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/polarcurves/">PolarCurves</a>.<a href="../../methods/itopolarcurveenumint-add/">Add</a> | <a href="../../collections/polarcurves/">PolarCurves</a>.<a href="../../methods/itopolarcurveenumint-copy/">Copy</a> | <a href="../../collections/polarcurves/">PolarCurves</a>.<a href="../../properties/itopolarcurveenumint-currcurve/">CurrCurve</a> | <a href="../../collections/polarcurves/">PolarCurves</a>.<a href="../../methods/itopolarcurveenumint-item/">Item</a> | <a href="../../collections/polarcurves/">PolarCurves</a>.<a href="../../properties/itopolarcurveenumint-leadingcurve/">LeadingCurve</a> | <a href="../../collections/polarcurves/">PolarCurves</a>.<a href="../../methods/itopolarcurveenumint-setleadingcurve/">SetLeadingCurve</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToPolarCurveInt.htm`*
