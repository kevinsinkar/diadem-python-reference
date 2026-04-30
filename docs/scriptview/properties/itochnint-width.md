---
title: "IToChnInt.Width"
description: "Specifies the column width in a 2D channel table in DIAdem VIEW, in pixel."
---

# IToChnInt.Width

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Width for Column

Specifies the column width in a 2D channel table in DIAdem VIEW, in pixel.

## Signature

```python
obj.Width
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The value -1 refers to the default column width.</td></tr></table>
</div>

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "ChannelTable"
oMyColumns = dd.View.Sheets(1).Areas(1).DisplayObj.Columns
oMyColumns.Add("[1]/[3]")
for oMyColumn in oMyColumns:
    oMyColumn.Width = oMyColumns(1).Width
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Width_IToChnInt.htm`*
