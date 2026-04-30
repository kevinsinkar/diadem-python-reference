---
title: "IToChannelTableInt.NumFormat"
description: "Specifies the numeric format for all the columns of a channel table in DIAdem VIEW."
---

# IToChannelTableInt.NumFormat

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: NumFormat for ChannelTable

Specifies the numeric format for all the columns of a channel table in DIAdem VIEW.

## Signature

```python
obj.NumFormat
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "ChannelTable"
oMyTable = dd.View.Sheets(1).Areas(1).DisplayObj
oMyTable.DynamicMode = "All"
oMyTable.NumFormat = "d.dd"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_NumFormat_IToChannelTableInt.htm`*
