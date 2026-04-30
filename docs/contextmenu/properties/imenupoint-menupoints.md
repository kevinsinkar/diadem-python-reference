---
title: "IMenuPoint.MenuPoints"
description: "Returns the items of a submenu."
---

# IMenuPoint.MenuPoints

!!! abstract "Property &middot; `ContextMenu.chm`"
    Property: MenuPoints for MenuPoint

Returns the items of a submenu.

## Signature

```python
return_value = obj.MenuPoints
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
    MenuPoints.RemoveAll()
    MenuPoints.Add("MenuPoint1", 1)
    MyMenuPoint = MenuPoints.Add("SubMenu", 2)
    MyMenuPoint.MenuPoints.Add("SubMenuPoint1", 3)
    MyMenuPoint.MenuPoints.Add("SubMenuPoint2", 4)

# --- For DIAdem-VIEW ------------------------------------------
AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu","MyViewOnShowingContextMenu")

def MyViewOnShowingContextMenu(Area, MenuPoints):
    MenuPoints.RemoveAll()
    MenuPoints.Add("MenuPoint1", 1)
    MyMenuPoint = MenuPoints.Add("SubMenu", 2)
    MyMenuPoint.MenuPoints.Add("SubMenuPoint1", 3)
    MyMenuPoint.MenuPoints.Add("SubMenuPoint2", 4)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ContextMenu/properties/ContextMenu_property_MenuPoints_IMenuPoint.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
