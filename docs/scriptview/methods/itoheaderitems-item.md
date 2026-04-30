---
title: "IToHeaderItems.Item"
description: "Returns the HeaderItem object associated with a specific name or index in DIAdem VIEW."
---

# IToHeaderItems.Item

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: Item for HeaderItems

Returns the HeaderItem object associated with a specific name or index in DIAdem VIEW.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
dd.MsgBoxDisp("Name of first HeaderItem: " + dd.View.ActiveSheet.ActiveArea.DisplayObj.HeaderItems.Item(1).Name)
dd.MsgBoxDisp("Name of first HeaderItem: " + dd.View.ActiveSheet.ActiveArea.DisplayObj.HeaderItems(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_Item_IToHeaderItems.htm`*
