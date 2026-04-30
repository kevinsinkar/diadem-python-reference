---
title: "OrderLines"
description: "The OrderLine object provides an order line in a cascade display in DIAdem VIEW. Use the OrderLines collection to delete order lines or to add new order lines."
---

# OrderLines

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: OrderLines

The OrderLine object provides an order line in a cascade display in DIAdem VIEW. Use the OrderLines collection to delete order lines or to add new order lines.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\cascade.tdm","TDM","")
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Cascade"
oMyDisplayObj = oMySheet.ActiveArea.DisplayObj
oMyCascadeCurve = oMyDisplayObj.CurvesCascade.AddCascade("[2]/[1]","[2]/[2]","[2]/[3]")
oMyCascadeCurve.OrderChannelName = "[1]/[11]"
for I in range( 1, 6+1):
    oMyCascadeCurve.OrderLines.Add(I)
    oMyCascadeCurve.OrderLines(I).Color = "blue"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itoorderlineenumint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itoorderlineenumint-add/">Add</a> | <a href="../../methods/itoorderlineenumint-item/">Item</a> | <a href="../../methods/itoorderlineenumint-remove/">Remove</a> | <a href="../../methods/itoorderlineenumint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itocascadecurveint/">WaterfallCurve</a>.<a href="../../properties/itocascadecurveint-orderlines/">OrderLines</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToOrderLineEnumInt.htm`*
