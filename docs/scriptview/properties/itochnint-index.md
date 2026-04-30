---
title: "IToChnInt.Index"
description: "Returns the index of a column in a channel table in DIAdem VIEW."
---

# IToChnInt.Index

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Index for Column

Returns the index of a column in a channel table in DIAdem VIEW.

## Signature

```python
obj.Index
```

## Python example

```python
oNewColumn = dd.View.ActiveSheet.ActiveArea.DisplayObj.Columns.Add("[1]/[3]")
dd.MsgBoxDisp("Index of oNewColumn: " + oNewColumn.Index)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Index_IToChnInt.htm`*
