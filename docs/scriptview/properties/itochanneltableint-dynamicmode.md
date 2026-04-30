---
title: "IToChannelTableInt.DynamicMode"
description: "Specifies which channels the channel table displays in DIAdem VIEW."
---

# IToChannelTableInt.DynamicMode

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: DynamicMode for ChannelTable

Specifies which channels the channel table displays in DIAdem VIEW.

## Signature

```python
obj.DynamicMode
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "ChannelTable"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.DynamicMode = "All"
oMyObj.HighLight = "Cols"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object Overview</a> |<a href="#" data-unresolved="1">Channel Table - Display</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_DynamicMode_IToChannelTableInt.htm`*
