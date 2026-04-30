---
title: "IToBodeCurveInt.AmplitudeChannelName"
description: "Specifies the name for an amplitude channel of a Bode curve in DIAdem VIEW."
---

# IToBodeCurveInt.AmplitudeChannelName

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: AmplitudeChannelName for BodeCurve

Specifies the name for an amplitude channel of a Bode curve in DIAdem VIEW.

## Signature

```python
obj.AmplitudeChannelName
```

## Python example

```python
dd.View.NewLayout()
dd.View.Sheets(1).Areas(1).DisplayObjType = "Bode"
oMyCurves = dd.View.Sheets(1).Areas(1).DisplayObj.CurvesBode
oMyCurve = oMyCurves.Add("[1]/[1]","[1]/[2]","[1]/[3]")
dd.MsgBoxDisp("X-channel: " + oMyCurve.XChannelName  + "\r\n" + "Phase: " + oMyCurve.PhaseChannelName  + "\r\n" + "Amplitude: " + oMyCurve.AmplitudeChannelName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_AmplitudeChannelName_IToBodeCurveInt.htm`*
