---
title: "IToChannelTableInt.ActiveColumn"
description: "Returns the active column of a channel table in DIAdem VIEW."
---

# IToChannelTableInt.ActiveColumn

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: ActiveColumn for ChannelTable

Returns the active column of a channel table in DIAdem VIEW.

## Signature

```python
obj.ActiveColumn
```

## Python example

```python
if dd.View.ActiveSheet.ActiveArea.DisplayObjType == "ChannelTable" :
    dd.MsgBoxDisp("Active column: " + dd.View.ActiveSheet.ActiveArea.DisplayObj.ActiveColumn)
else:
    dd.MsgBoxDisp("Area type: " + dd.View.ActiveSheet.ActiveArea.DisplayObjType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_ActiveColumn_IToChannelTableInt.htm`*
