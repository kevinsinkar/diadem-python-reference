---
title: "IToSubCursorSidebandInt.Sidebands"
description: "Returns the additional cursor lines of a sideband cursor in a 2D axis system in DIAdem VIEW as an object."
---

# IToSubCursorSidebandInt.Sidebands

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Sidebands for SidebandCursor

Returns the additional cursor lines of a sideband cursor in a 2D axis system in DIAdem VIEW as an object.

## Signature

```python
return_value = obj.Sidebands
```

## Python example

```python
oMyObj = dd.View.ActiveSheet.ActiveArea
if oMyObj.DisplayObjType == "CurveChart2D" :
    oMyObj.DisplayObj.SubCursorType = dd.eVIEWSubCursorTypeSideband
    dd.MsgBoxDisp("Addional cursor lines: " + oMyObj.DisplayObj.SubCursor.Sidebands.Count + "\r\n" + "Line distance: " + oMyObj.DisplayObj.SubCursor.Sidebands.Interval)
else:
    dd.MsgBoxDisp(oMyObj.DisplayObjType + " Area")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Sidebands_IToSubCursorSidebandInt.htm`*
