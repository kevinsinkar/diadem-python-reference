---
title: "LegendItems"
description: "The LegendItems object provides a collection of the Legend entries of an axis system or a contour display in DIAdem VIEW. Use the LegendItems collection to dele"
---

# LegendItems

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: LegendItems

The LegendItems object provides a collection of the Legend entries of an axis system or a contour display in DIAdem VIEW. Use the LegendItems collection to delete legend items or to add new legend items.

## Python example

```python
oMyLegends = dd.View.ActiveSheet.ActiveArea.DisplayObj.LegendItems
sOutput = "Names of legend items: " + "\r\n"
for oMyLegendItem in oMyLegends:
    sOutput = sOutput + oMyLegendItem.Name + "\r\n"
print(sOutput)
```

```python
oMyLegend1 = dd.View.ActiveSheet.ActiveArea.DisplayObj.LegendItems.Add("CursorX")
oMyLegend1.Format ="d.dd"
```

```python
oMyLegend2 = dd.View.ActiveSheet.ActiveArea.DisplayObj.LegendItems.Add("Length")
oMyLegend2.Format = "d"
```

```python
oMyLegend3 = dd.View.ActiveSheet.ActiveArea.DisplayObj.LegendItems.Add("<freetext>")
oMyLegend3.Title = "Free Text"
oMyLegend3.Format = "Any descriptive text"
```

```python
oMyLegend4 = dd.View.ActiveSheet.ActiveArea.DisplayObj.LegendItems.Add("<freetext>")
oMyLegend4.Title = "Current Date"
oMyLegend4.Format = "Date: @CurrDate@"
```

```python
oMyLegend5 = dd.View.ActiveSheet.ActiveArea.DisplayObj.LegendItems.Add("<freetext>")
oMyLegend5.Title = "Y difference"
oMyLegend5.Format = "@@CurrentYDiff@@"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itoattrenumint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itoattrenumint-add/">Add</a> | <a href="../../methods/itoattrenumint-item/">Item</a> | <a href="../../methods/itoattrenumint-remove/">Remove</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itobodechartint/">Bode</a>.<a href="../../properties/itobodechartint-legenditems/">LegendItems</a> | <a href="../../objects/itocascadechartint/">Cascade</a>.<a href="../../properties/itocascadechartint-legenditems/">LegendItems</a> | <a href="../../objects/itocontourchartint/">Contour</a>.<a href="../../properties/itocontourchartint-legenditems/">LegendItems</a> | <a href="../../objects/ito2dchartint/">CurveChart2D</a>.<a href="../../properties/ito2dchartint-legenditems/">LegendItems</a> | <a href="../../objects/itoorbitchartint/">Orbit</a>.<a href="../../properties/itoorbitchartint-legenditems/">LegendItems</a> | <a href="../../objects/itopolarchartint/">Polar</a>.<a href="../../properties/itopolarchartint-legenditems/">LegendItems</a> | <a href="../../objects/itoshaftcenterlinechartint/">ShaftCenterline</a>.<a href="../../properties/itoshaftcenterlinechartint-legenditems/">LegendItems</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Analyzing and Displaying Channels Section by Section</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Background Segments in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Show texts of assignment channels in the VIEW legend</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToAttrEnumInt.htm`*
