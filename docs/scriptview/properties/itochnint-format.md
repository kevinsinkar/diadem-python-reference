---
title: "IToChnInt.Format"
description: "Specifies the Format definition of the texts and numbers in a channel table in DIAdem VIEW."
---

# IToChnInt.Format

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Format for Column

Specifies the Format definition of the texts and numbers in a channel table in DIAdem VIEW.

## Signature

```python
obj.Format
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "ChannelTable"
dd.View.Sheets(1).Areas(1).DisplayObj.Columns.Add("[1]/[1]")
for oColumn in dd.View.Sheets(1).Areas(1).DisplayObj.Columns:
    oColumn.Format = "d.dd"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Format Numbers</a> | <a href="#" data-unresolved="1">Object Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Format_IToChnInt.htm`*
