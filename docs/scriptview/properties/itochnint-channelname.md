---
title: "IToChnInt.ChannelName"
description: "Specifies the name of a channel in a column of the channel table in DIAdem VIEW."
---

# IToChnInt.ChannelName

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: ChannelName for Column

Specifies the name of a channel in a column of the channel table in DIAdem VIEW.

## Signature

```python
obj.ChannelName
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "ChannelTable"
oMyColumns = dd.View.Sheets(1).Areas(1).DisplayObj.Columns
oMyColumns.Add("[1]/[3]")
for oMyColumn in oMyColumns:
    dd.MsgBoxDisp(oMyColumn.ChannelName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_ChannelName_IToChnInt.htm`*
