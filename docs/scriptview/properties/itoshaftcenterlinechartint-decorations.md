---
title: "IToShaftCenterlineChartInt.Decorations"
description: "Specifies text or graphics displayed as decorations in a shaft centerline axis system in DIAdem VIEW."
---

# IToShaftCenterlineChartInt.Decorations

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Decorations for ShaftCenterline

Specifies text or graphics displayed as decorations in a shaft centerline axis system in DIAdem VIEW.

## Signature

```python
return_value = obj.Decorations
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "ShaftCenterline"
oMyChart = dd.View.Sheets(1).Areas(1).DisplayObj
oMyCurve = oMyChart.CurvesShaftCenterline.Add("[2]/[1]","[2]/[2]")

oMyDecoration = oMyChart.Decorations.Add(dd.eVIEWDecorationTypeText,"Decoration")
oMyDecoration.Text = "DecorationText"
oMyDecoration.PositionHorizontal = dd.eVIEWDecorationPosHorizontalLeft
oMyDecoration.PositionVertical = dd.eVIEWDecorationPosVerticalTop
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Decorations_IToShaftCenterlineChartInt.htm`*
