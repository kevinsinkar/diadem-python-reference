---
title: "IToContourCurveBaseInt.TagTemporary"
description: "Specifies a temporary tag for a curve in a contour display in DIAdem VIEW."
---

# IToContourCurveBaseInt.TagTemporary

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: TagTemporary for ContourCurveBase

Specifies a temporary tag for a curve in a contour display in DIAdem VIEW.

## Signature

```python
obj.TagTemporary
```

## Python example

```python
class TempTag:
    Name = ""
    IsValid = 0

dd.View.Sheets.Add("NewContour")
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "Contour"
oMyCurves = dd.View.ActiveSheet.ActiveArea.DisplayObj.CurvesContour
oMyCurve = oMyCurves.AddContour("[1]/[1]","[1]/[2]","{1]/[3]")
oMyCurves.AddIsoline("[1]/[1]","[1]/[4]")
oMyCurve.TagTemporary = TempTag()
oMyCurve.TagTemporary.Name = "Contour"
oMyCurve.TagTemporary.IsValid = 1
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_TagTemporary_IToContourCurveBaseInt.htm`*
