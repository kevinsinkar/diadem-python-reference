---
title: "IMenuPoints.RemoveAll"
description: "Removes all items from the context menu."
---

# IMenuPoints.RemoveAll

!!! abstract "Method &middot; `ContextMenu.chm`"
    Method: RemoveAll for MenuPoints

Removes all items from the context menu.

## Signature

```python
obj.RemoveAll
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
dd.AddUserCommandToEvent("dd.Navigator.Events.OnShowingContextMenu", "MyNavigatorOnShowingContextMenu")
dd.AddUserCommandToEvent("dd.Navigator.Events.OnContextMenuPointSelected","MyNavigatorOnContextMenuPointSelected")

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ContextMenu/methods/ContextMenu_method_RemoveAll_IMenuPoints.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
