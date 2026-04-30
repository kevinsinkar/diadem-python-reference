---
title: "IMenuPoint.Enable"
description: "Specifies whether DIAdem disables a context menu item."
---

# IMenuPoint.Enable

!!! abstract "Property &middot; `ContextMenu.chm`"
    Property: Enable for MenuPoint

Specifies whether DIAdem disables a context menu item.

## Signature

```python
obj.Enable
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
    for MenuPoint in MenuPoints:
        MenuPoint.Enable(FALSE)

# --- For DIAdem-VIEW ------------------------------------------
AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu","MyViewOnShowingContextMenu")

def MyViewOnShowingContextMenu(Area, MenuPoints):
    for MenuPoint in MenuPoints:
        MenuPoint.Enable(FALSE)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ContextMenu/properties/ContextMenu_property_Enable_IMenuPoint.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
