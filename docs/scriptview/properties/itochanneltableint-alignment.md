---
title: "IToChannelTableInt.Alignment"
description: "Specifies the alignment of the text in a channel table in DIAdem VIEW."
---

# IToChannelTableInt.Alignment

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Alignment for ChannelTable

Specifies the alignment of the text in a channel table in DIAdem VIEW.

## Signature

```python
obj.Alignment
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "ChannelTable"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.Columns.Add("[1]/[1]")
oMyObj.Alignment = "Center"
dd.View.AutoRefresh = True
dd.View.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Alignment_IToChannelTableInt.htm`*
