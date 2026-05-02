---
title: "IMenuPoint.ID"
description: "Specifies the ID of a context menu item. Use the ID to determine which action DIAdem executes in the OnContextMenuPointSelected event."
---

# IMenuPoint.ID

!!! abstract "Property &middot; `ContextMenu.chm`"
    Property: ID for MenuPoint

Specifies the ID of a context menu item. Use the ID to determine which action DIAdem executes in the OnContextMenuPointSelected event.

## Signature

```python
obj.ID
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>Assign only values less than 22000 to an ID.</td>
</tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>To test the following example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
# --- For DIAdem-NAVIGATOR ------------------------------------------
dd.AddUserCommandToEvent("dd.Navigator.Events.OnShowingContextMenu", "MyOnShowingContextMenu")
dd.AddUserCommandToEvent("dd.Navigator.Events.OnContextMenuPointSelected","MyOnContextMenuPointSelected")

def MyNavigatorOnShowingContextMenu(ParentObj, MenuPoints):
    MenuPoints.RemoveAll
    MenuPoints.Add("MyMenuPoint1", 1)
    MenuPoints.Add("MyMenuPoint2", 2)
    MenuPoints.Add("MyMenuPoint3", 3)
    MenuPoints.Remove(3)

def MyNavigatorOnContextMenuPointSelected(ParentObj, MenuPoint):
    pass
    # select MenuPoint.ID
    # case 1    MsgBoxDisp("DIAdem-NAVIGATOR: MyMenuPoint1 selected")
    # case 2    MsgBoxDisp("DIAdem-NAVIGATOR: MyMenuPoint2 selected")

# --- For DIAdem-VIEW ------------------------------------------
dd.AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu", "MyViewOnShowingContextMenu")
dd.AddUserCommandToEvent("dd.View.Events.OnContextMenuPointSelected","MyViewOnContextMenuPointSelected")

def MyViewOnShowingContextMenu(Area, MenuPoints):
    MenuPoints.RemoveAll
    MenuPoints.Add("MyMenuPoint1", 1)
    MenuPoints.Add("MyMenuPoint2", 2)
    MenuPoints.Add("MyMenuPoint3", 3)
    MenuPoints.Remove(3)

def MyViewOnContextMenuPointSelected(Area, MenuPoint):
    pass
    # select MenuPoint.ID
    # case 1    MsgBoxDisp("DIAdem-VIEW: MyMenuPoint1 selected")
    # case 2    MsgBoxDisp("DIAdem-VIEW: MyMenuPoint2 selected")
```

---

*Source: `ContextMenu/properties/ContextMenu_property_ID_IMenuPoint.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
