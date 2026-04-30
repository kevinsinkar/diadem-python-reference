---
title: "IToBodeChartInt.ActiveSystem"
description: "Returns the active axis system of a Bode axis system in DIAdem VIEW."
---

# IToBodeChartInt.ActiveSystem

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: ActiveSystem for Bode

Returns the active axis system of a Bode axis system in DIAdem VIEW.

## Signature

```python
obj.ActiveSystem
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eVIEWBodeSystemPhase` | 0 | Phase axis system |
| `eVIEWBodeSystemAmplitude` | 1 | Amplitude axis system |

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "Bode"
oMyViewObj = dd.View.ActiveSheet.ActiveArea.DisplayObj.CurvesBode
oMyViewObj.Add("[2]/[1]","[2]/[2]","[2]/[3]")
dd.MsgBoxDisp("Active system: " + dd.View.ActiveSheet.ActiveArea.DisplayObj.ActiveSystem)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_ActiveSystem_IToBodeChartInt.htm`*
