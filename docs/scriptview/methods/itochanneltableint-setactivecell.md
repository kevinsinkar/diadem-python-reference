---
title: "IToChannelTableInt.SetActiveCell"
description: "Moves the entry marker to the specified position in a 2D channel table in DIAdem VIEW."
---

# IToChannelTableInt.SetActiveCell

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: SetActiveCell for ChannelTable

Moves the entry marker to the specified position in a 2D channel table in DIAdem VIEW.

## Signature

```python
obj.SetActiveCell(RowIndex, ColIndex)
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "ChannelTable"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.Columns.Add("[1]/[3]")
oMyObj.SetActiveCell(1,1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_SetActiveCell_IToChannelTableInt.htm`*
