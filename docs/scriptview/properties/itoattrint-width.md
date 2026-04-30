---
title: "IToAttrInt.Width"
description: "Specifies the column width of a legend entry in a 2D axis system in DIAdem VIEW."
---

# IToAttrInt.Width

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Width for LegendItem

Specifies the column width of a legend entry in a 2D axis system in DIAdem VIEW.

## Signature

```python
obj.Width
```

## Python example

```python
oMyLegends = dd.View.ActiveSheet.ActiveArea.DisplayObj.LegendItems
for oMyLegendItem in oMyLegends:
    dd.MsgBoxDisp("Width of LegendItem: " + oMyLegendItem.Width)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Width_IToAttrInt.htm`*
