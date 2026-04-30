---
title: "ITo2DCurveEnumInt.CurrCurve"
description: "Returns the curve of a 2D axis system of DIAdem VIEW with the legend that includes the formula expression which uses this property."
---

# ITo2DCurveEnumInt.CurrCurve

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: CurrCurve for 2DCurves

Returns the curve of a 2D axis system of DIAdem VIEW with the legend that includes the formula expression which uses this property.

## Signature

```python
return_value = obj.CurrCurve
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>You only can use this property in a user command, or as a legend expression in a script expression. Enclose the legend expression in @@ characters.</td></tr></table>
</div>

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyChart = dd.View.ActiveSheet.ActiveArea.DisplayObj

oMyCurve = oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
oMyCurve.MarkerType = "square"

oMyLegend = oMyChart.LegendItems.Add("<freetext>")
oMyLegend.Title = "Marker interval"
oMyLegend.Format = "@@View.CurrSheet.CurrArea.DisplayObj.Curves2D.CurrCurve.MarkerIntervalPoints@@"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_CurrCurve_ITo2DCurveEnumInt.htm`*
