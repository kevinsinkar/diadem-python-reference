---
title: "IMenuPoints.Add"
description: "Adds a new item to the context menu or the submenu."
---

# IMenuPoints.Add

!!! abstract "Method &middot; `ContextMenu.chm`"
    Method: Add for MenuPoints

Adds a new item to the context menu or the submenu.

## Signature

```python
return_value = obj.Add(Name, ID)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  To test the following example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <b>Settings»Extensions»User Commands.</b></td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
AddUserCommandToEvent("dd.Navigator.Events.OnShowingContextMenu", "MyNavigatorOnShowingContextMenu")
AddUserCommandToEvent("dd.Navigator.Events.OnContextMenuPointSelected","MyNavigatorOnContextMenuPointSelected")

def MyNavigatorOnShowingContextMenu(ParentObj, MenuPoints):
    MenuPoints.RemoveAll
    MenuPoints.Add("MyMenuPoint1", 1)
    MenuPoints.Add("", 0)  ' Separator
    oMyMenuPoint = MenuPoints.Add("Main", 2) 'Main entry
    oMyMenuPoint.MenuPoints.Add("SubMenupoint21", 21) 'Sub entry
    oMyMenuPoint.MenuPoints.Add("SubMenupoint22", 22) 'Sub entry

def MyNavigatorOnContextMenuPointSelected(ParentObj, MenuPoint):
    # select MenuPoint.ID
    # case 1    dd.MsgBox("DIAdem-NAVIGATOR: MyMenuPoint1 selected")
    # case 2    dd.MsgBox("DIAdem-NAVIGATOR: MyMenuPoint2 selected")
    # case 21   dd.MsgBox("DIAdem-NAVIGATOR: MyMenuPoint21 selected")
    # case 22   dd.MsgBox("DIAdem-NAVIGATOR: MyMenuPoint22 selected")

# --- For DIAdem-VIEW ------------------------------------------
AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu", "MyViewOnShowingContextMenu")
AddUserCommandToEvent("dd.View.Events.OnContextMenuPointSelected","MyViewOnContextMenuPointSelected")

def MyViewOnShowingContextMenu(Area, MenuPoints):
    MenuPoints.RemoveAll
    MenuPoints.Add("MyMenuPoint1", 1)
    MenuPoints.Add("MyMenuPoint2", 2)

def MyViewOnContextMenuPointSelected(Area, MenuPoint):
    # select MenuPoint.ID
    # case 1    dd.MsgBox("DIAdem-VIEW: MyMenuPoint1 selected")
    # case 2    dd.MsgBox("DIAdem-VIEW: MyMenuPoint2 selected")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ContextMenu/methods/ContextMenu_method_Add_IMenuPoints.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
