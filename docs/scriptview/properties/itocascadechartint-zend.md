---
title: "IToCascadeChartInt.ZEnd"
description: "Returns the end of the value range of the track axis of a cascade display in DIAdem VIEW."
---

# IToCascadeChartInt.ZEnd

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: ZEnd for Cascade

Returns the end of the value range of the track axis of a cascade display in DIAdem VIEW.

## Signature

```python
obj.ZEnd
```

## Python example

```python
if dd.View.ActiveSheet.ActiveArea.DisplayObjType == "Cascade" :
    oMyChart = dd.View.ActiveSheet.ActiveArea.DisplayObj
    dd.LogfileWrite("XBegin: " + dd.Str(oMyChart.XBegin) + "\r\n" + "XEnd: " + dd.Str(oMyChart.XEnd) + "\r\n" +"YBegin: " + dd.Str(oMyChart.YBegin) + "\r\n" + "YEnd: " + dd.Str(oMyChart.YEnd) + "\r\n" +"ZBegin: " + dd.Str(oMyChart.ZBegin) + "\r\n" + "ZEnd: " + dd.Str(oMyChart.ZEnd))
else:
    dd.MsgBoxDisp("No Cascade area")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_ZEnd_IToCascadeChartInt.htm`*
