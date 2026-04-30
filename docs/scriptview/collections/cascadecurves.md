---
title: "CascadeCurves"
description: "The CascadeCurves object provides access to a waterfall curve in a cascade display in DIAdem VIEW. Use the Line object to define the display of the order line."
---

# CascadeCurves

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: CascadeCurves

The CascadeCurves object provides access to a waterfall curve in a cascade display in DIAdem VIEW. Use the Line object to define the display of the order line.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\cascade.tdm","TDM","")
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Cascade"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyChart.CurvesCascade.AddCascade("[2]/[1]","[2]/[2]","[2]/[3]")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itocascadecurveenumint-count/">Count</a> | <a href="../../properties/itocascadecurveenumint-currcurve/">CurrCurve</a> | <a href="../../properties/itocascadecurveenumint-leadingcurve/">LeadingCurve</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itocascadecurveenumint-addcascade/">AddCascade</a> | <a href="../../methods/itocascadecurveenumint-addline/">AddLine</a> | <a href="../../methods/itocascadecurveenumint-item/">Item</a> | <a href="../../methods/itocascadecurveenumint-remove/">Remove</a> | <a href="../../methods/itocascadecurveenumint-removeall/">RemoveAll</a> | <a href="../../methods/itocascadecurveenumint-setleadingcurve/">SetLeadingCurve</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itocascadechartint/">Cascade</a>.<a href="../../properties/itocascadechartint-curvescascade/">CurvesCascade</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToCascadeCurveEnumInt.htm`*
