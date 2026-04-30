---
title: "ITo2DChartInt.XScalingMode"
description: "Specifies the zoom mode and the scroll mode in a 2D axis system in DIAdem VIEW."
---

# ITo2DChartInt.XScalingMode

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: XScalingMode for CurveChart2D

Specifies the zoom mode and the scroll mode in a 2D axis system in DIAdem VIEW.

## Signature

```python
obj.XScalingMode
```

## Notes

<div markdown="1">
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">XScalingMode</span> property replaces the <span class="Monospace">XScaling</span> property.</td></tr></table>
</div>

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "CurveChart2D"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.Curves2D.Add("[2]/[1]","[2]/[2]")
dd.View.Sheets(1).Cursor.X1 = 10
dd.View.Sheets(1).Cursor.X2 = 40
dd.View.Sheets(1).Areas(1).DisplayObj.XScalingMode = "RangeZoom"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Creating a Python Graphic with a Pie Chart in VIEW</a> | <a href="#" data-unresolved="1">Creating Areas</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Generating and Formatting Text</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Moving or Copying Areas</a> | <a href="#" data-unresolved="1">Partitioning Worksheets</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_XScalingMode_ITo2DChartInt.htm`*
