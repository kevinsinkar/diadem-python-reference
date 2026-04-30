---
title: "IToShaftCenterlineCurveInt"
description: "The ShaftCenterlineCurve object provides access to a curve in a shaft centerline axis system in DIAdem VIEW. Use the ShaftCenterlineCurve object to specify the "
---

# IToShaftCenterlineCurveInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: ShaftCenterlineCurve

The ShaftCenterlineCurve object provides access to a curve in a shaft centerline axis system in DIAdem VIEW. Use the ShaftCenterlineCurve object to specify the curve properties.

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
<p><a href="../../properties/itoshaftcenterlinecurveint-color/">Color</a> | <a href="../../properties/itoshaftcenterlinecurveint-colorrgb/">ColorRGB</a> | <a href="../../properties/itoshaftcenterlinecurveint-enable/">Enable</a> | <a href="../../properties/itoshaftcenterlinecurveint-index/">Index</a> | <a href="../../properties/itoshaftcenterlinecurveint-isvalid/">IsValid</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelatbegin/">LabelAtBegin</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelatend/">LabelAtEnd</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelchannelname/">LabelChannelName</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelchannelorientation/">LabelChannelOrientation</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelcolor/">LabelColor</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelcolorauto/">LabelColorAuto</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelcolorrgb/">LabelColorRGB</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelindexchannelname/">LabelIndexChannelName</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelintervallength/">LabelIntervalLength</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelintervalpoints/">LabelIntervalPoints</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelmode/">LabelMode</a> | <a href="../../properties/itoshaftcenterlinecurveint-labelrepetitionmode/">LabelRepetitionMode</a> | <a href="../../properties/itoshaftcenterlinecurveint-labeltext/">LabelText</a> | <a href="../../properties/itoshaftcenterlinecurveint-markeratbegin/">MarkerAtBegin</a> | <a href="../../properties/itoshaftcenterlinecurveint-markeratend/">MarkerAtEnd</a> | <a href="../../properties/itoshaftcenterlinecurveint-markercolor/">MarkerColor</a> | <a href="../../properties/itoshaftcenterlinecurveint-markercolorauto/">MarkerColorAuto</a> | <a href="../../properties/itoshaftcenterlinecurveint-markercolorrgb/">MarkerColorRGB</a> | <a href="../../properties/itoshaftcenterlinecurveint-markerfillcolor/">MarkerFillColor</a> | <a href="../../properties/itoshaftcenterlinecurveint-markerfillcolorauto/">MarkerFillColorAuto</a> | <a href="../../properties/itoshaftcenterlinecurveint-markerfillcolorrgb/">MarkerFillColorRGB</a> | <a href="../../properties/itoshaftcenterlinecurveint-markerfrequencymode/">MarkerFrequencyMode</a> | <a href="../../properties/itoshaftcenterlinecurveint-markerintervallength/">MarkerIntervalLength</a> | <a href="../../properties/itoshaftcenterlinecurveint-markerintervalpoints/">MarkerIntervalPoints</a> | <a href="../../properties/itoshaftcenterlinecurveint-markerlinewidth/">MarkerLineWidth</a> | <a href="../../properties/itoshaftcenterlinecurveint-markersize/">MarkerSize</a> | <a href="../../properties/itoshaftcenterlinecurveint-markertype/">MarkerType</a> | <a href="../../properties/itoshaftcenterlinecurveint-name/">Name</a> | <a href="../../properties/itoshaftcenterlinecurveint-selected/">Selected</a> | <a href="../../properties/itoshaftcenterlinecurveint-tagstored/">TagStored</a> | <a href="../../properties/itoshaftcenterlinecurveint-tagtemporary/">TagTemporary</a> | <a href="../../properties/itoshaftcenterlinecurveint-type/">Type</a> | <a href="../../properties/itoshaftcenterlinecurveint-visibleinlegend/">VisibleInLegend</a> | <a href="../../properties/itoshaftcenterlinecurveint-xchannelname/">XChannelName</a> | <a href="../../properties/itoshaftcenterlinecurveint-ychannelname/">YChannelName</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/shaftcenterlinecurves/">ShaftCenterlineCurves</a>.<a href="../../methods/itoshaftcenterlinecurveenumint-add/">Add</a> | <a href="../../collections/shaftcenterlinecurves/">ShaftCenterlineCurves</a>.<a href="../../methods/itoshaftcenterlinecurveenumint-copy/">Copy</a> | <a href="../../collections/shaftcenterlinecurves/">ShaftCenterlineCurves</a>.<a href="../../properties/itoshaftcenterlinecurveenumint-currcurve/">CurrCurve</a> | <a href="../../collections/shaftcenterlinecurves/">ShaftCenterlineCurves</a>.<a href="../../methods/itoshaftcenterlinecurveenumint-item/">Item</a> | <a href="../../collections/shaftcenterlinecurves/">ShaftCenterlineCurves</a>.<a href="../../properties/itoshaftcenterlinecurveenumint-leadingcurve/">LeadingCurve</a> | <a href="../../collections/shaftcenterlinecurves/">ShaftCenterlineCurves</a>.<a href="../../methods/itoshaftcenterlinecurveenumint-setleadingcurve/">SetLeadingCurve</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToShaftCenterlineCurveInt.htm`*
