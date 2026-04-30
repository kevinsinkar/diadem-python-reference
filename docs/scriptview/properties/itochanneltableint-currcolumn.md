---
title: "IToChannelTableInt.CurrColumn"
description: "Returns the column of a DIAdem VIEW channel table whose legend includes the formula expression that uses this property."
---

# IToChannelTableInt.CurrColumn

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: CurrColumn for ChannelTable

Returns the column of a DIAdem VIEW channel table whose legend includes the formula expression that uses this property.

## Signature

```python
return_value = obj.CurrColumn
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "ChannelTable"
MyChnTab = dd.View.Sheets(1).Areas(1).DisplayObj
MyChnTab.Columns.Add("[1]/[1]")
MyChnTab.Columns.Add("[1]/[2]")
MyChnTab.Columns.Add("[1]/[3]")

oMyProps = MyChnTab.HeaderItems.Add("<freetext>")
oMyProps.Title = "ArithMean"
oMyProps.Format ="@@CCh(View.CurrSheet.CurrArea.DisplayObj.CurrColumn.ChannelNumber,0)@@"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Creating a Python Graphic with a Pie Chart in VIEW</a> | <a href="#" data-unresolved="1">Creating Areas</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Generating and Formatting Text</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Moving or Copying Areas</a> | <a href="#" data-unresolved="1">Partitioning Worksheets</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_CurrColumn_IToChannelTableInt.htm`*
