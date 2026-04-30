---
title: "IMenuPoints.Item"
description: "Returns the context menu item for a certain index."
---

# IMenuPoints.Item

!!! abstract "Method &middot; `ContextMenu.chm`"
    Method: Item for MenuPoints

Returns the context menu item for a certain index.

## Signature

```python
return_value = obj.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  To test the following example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands.</strong></td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
# --- For DIAdem-NAVIGATOR ------------------------------------------
AddUserCommandToEvent("dd.Navigator.Events.OnShowingContextMenu","MyNavigatorOnShowingContextMenu")

def MyNavigatorOnShowingContextMenu(ParentObj, MenuPoints):
    for Index in range(1, MenuPoints.Count + 1):
        MenuPoints.Item(Index).Enable(False)

# --- For DIAdem-VIEW ------------------------------------------
AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu","MyViewOnShowingContextMenu")

def MyViewOnShowingContextMenu(Area, MenuPoints):
    for Index in range(1, MenuPoints.Count + 1):
        MenuPoints.Item(Index).Enable(False)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ContextMenu/methods/ContextMenu_method_Item_IMenuPoints.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
