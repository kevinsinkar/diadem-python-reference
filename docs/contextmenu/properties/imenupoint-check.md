---
title: "IMenuPoint.Check"
description: "Specifies whether a context menu item is active. DIAdem identifies the enabled items with a tick in front of the item."
---

# IMenuPoint.Check

!!! abstract "Property &middot; `ContextMenu.chm`"
    Property: Check for MenuPoint

Specifies whether a context menu item is active. DIAdem identifies the enabled items with a tick in front of the item.

## Signature

```python
obj.Check
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>To test the following example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
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
    MenuPoints.Add("MyMenuPoint1", 1).Check = TRUE

# --- For DIAdem-VIEW ------------------------------------------
AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu","MyViewOnShowingContextMenu")

def MyViewOnShowingContextMenu(Area, MenuPoints):
    MenuPoints.Add("MyMenuPoint1", 1).Check = TRUE
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ContextMenu/properties/ContextMenu_property_Check_IMenuPoint.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
