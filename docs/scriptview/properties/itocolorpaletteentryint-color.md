---
title: "IToColorPaletteEntryInt.Color"
description: "Specifies the palette color DIAdem uses for a contour display or a bird's eye view display. The value range of the property and the value range of the ColorLst "
---

# IToColorPaletteEntryInt.Color

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Color for ColorPaletteEntry

Specifies the palette color DIAdem uses for a contour display or a bird's eye view display. The value range of the property and the value range of the ColorLst variable are identical.

## Signature

```python
obj.Color
```

## Python example

```python
if dd.View.ActiveSheet.ActiveArea.DisplayObjType == "Contour" :
    oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj.UserDefinedColoringEntries
    for i in range( 1, oMyObj.Count+1):
        dd.LogfileWrite("Color: " + oMyObj(i).Color + ", ColorRGB: " + oMyObj(i).ColorRGB + ", Value: " + oMyObj(i).Value)
```

```python
if dd.View.ActiveSheet.ActiveArea.DisplayObjType == "BirdsEyeView" :
    oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj.BirdsEyeViewObjects(1).UserDefinedColoringEntries
    for i in range( 1, oMyObj.Count+1):
        dd.LogfileWrite("Color: " + oMyObj(i).Color + ", ColorRGB: " + oMyObj(i).ColorRGB + ", Value: " + oMyObj(i).Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Creating a Python Graphic with a Pie Chart in VIEW</a> | <a href="#" data-unresolved="1">Creating Areas</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Generating and Formatting Text</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Moving or Copying Areas</a> | <a href="#" data-unresolved="1">Partitioning Worksheets</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Color_IToColorPaletteEntryInt.htm`*
