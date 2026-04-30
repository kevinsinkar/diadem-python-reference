---
title: "IToChannelTableInt.IndexColumnWidth"
description: "Specifies the index column width in a channel table in DIAdem VIEW."
---

# IToChannelTableInt.IndexColumnWidth

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: IndexColumnWidth for ChannelTable

Specifies the index column width in a channel table in DIAdem VIEW.

## Signature

```python
obj.IndexColumnWidth
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "ChannelTable"
oMyObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyObj.Columns.Add("[1]/[3]")
oMyObj.IndexColumnWidth = oMyObj.Columns(1).ColumnWidth
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_IndexColumnWidth_IToChannelTableInt.htm`*
