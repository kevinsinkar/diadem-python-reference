---
title: "IToChannelTableInt.DynamicModeGroupName"
description: "Specifies the group of the channels that the channel table displays in DIAdem VIEW."
---

# IToChannelTableInt.DynamicModeGroupName

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: DynamicModeGroupName for ChannelTable

Specifies the group of the channels that the channel table displays in DIAdem VIEW.

## Signature

```python
obj.DynamicModeGroupName
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>If the <span class="Monospace">DynamicModeGroupName</span> property contains an empty string, the channel table displays all the channels of the default group.</td></tr></table>
</div>

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "ChannelTable"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.DynamicMode = "Group"
oMyObj.DynamicModeGroupName = "Noise"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object Overview</a> |<a href="#" data-unresolved="1">Channel Table - Display</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_DynamicModeGroupName_IToChannelTableInt.htm`*
