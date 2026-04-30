---
title: "IMenuPoint.Tag"
description: "Contains additional information about the properties of a context menu item. Use the Tag property in the OnContextMenuPointSelected event."
---

# IMenuPoint.Tag

!!! abstract "Property &middot; `ContextMenu.chm`"
    Property: Tag for MenuPoint

Contains additional information about the properties of a context menu item. Use the Tag property in the OnContextMenuPointSelected event.

## Signature

```python
obj.Tag
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
AddUserCommandToEvent("dd.Navigator.Events.OnShowingContextMenu", "MyNavigatorOnShowingContextMenu")
AddUserCommandToEvent("dd.Navigator.Events.OnContextMenuPointSelected","MyNavigatorOnContextMenuPointSelected")

def MyNavigatorSub():
    MsgBoxDisp("MySub was selected")

def MyNavigatorOnShowingContextMenu(ParentObj, MenuPoints):
    oMyMenuPoint = MenuPoints.Add("Execute MySub", 1)
    oMyMenuPoint.Tag = "MyNavigatorSub"

def MyNavigatorOnContextMenuPointSelected(ParentObj, MenuPoint):
    Execute MenuPoint.Tag

# --- For DIAdem-VIEW ------------------------------------------
AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu", "MyViewOnShowingContextMenu")
AddUserCommandToEvent("dd.View.Events.OnContextMenuPointSelected","MyViewOnContextMenuPointSelected")

def MyViewSub():
    MsgBoxDisp("MySub was selected")

def MyViewOnShowingContextMenu(Area, MenuPoints):
    oMyMenuPoint = MenuPoints.Add("Execute MySub", 1)
    oMyMenuPoint.Tag = "MyViewSub"

def MyViewOnContextMenuPointSelected(Area, MenuPoint):
    Execute MenuPoint.Tag
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ContextMenu/properties/ContextMenu_property_Tag_IMenuPoint.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
