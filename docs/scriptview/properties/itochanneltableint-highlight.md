---
title: "IToChannelTableInt.Highlight"
description: "Specifies whether the channel table highlights rows or columns in DIAdem VIEW."
---

# IToChannelTableInt.Highlight

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Highlight for ChannelTable

Specifies whether the channel table highlights rows or columns in DIAdem VIEW.

## Signature

```python
obj.Highlight
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "ChannelTable"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.DynamicMode = "All"
oMyObj.Highlight = "Cols"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Highlight_IToChannelTableInt.htm`*
