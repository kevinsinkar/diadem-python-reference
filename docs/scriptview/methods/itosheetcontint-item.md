---
title: "IToSheetContInt.Item"
description: "Returns the Sheet object associated with a specific name or index in DIAdem VIEW."
---

# IToSheetContInt.Item

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: Item for Sheets

Returns the Sheet object associated with a specific name or index in DIAdem VIEW.

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
dd.MsgBoxDisp("Name of first sheet: " + dd.View.Sheets.Item(1).Name)
dd.MsgBoxDisp("Name of first sheet: " + dd.View.Sheets(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_Item_IToSheetContInt.htm`*
