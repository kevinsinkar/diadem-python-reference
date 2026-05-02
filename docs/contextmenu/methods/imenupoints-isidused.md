---
title: "IMenuPoints.IsIDUsed"
description: "Investigates, whether an item from the context menu is using a specific ID."
---

# IMenuPoints.IsIDUsed

!!! abstract "Method &middot; `ContextMenu.chm`"
    Method: IsIDUsed for MenuPoints

Investigates, whether an item from the context menu is using a specific ID.

## Signature

```python
bIsIDUsed = Object.IsIDUsed(ID)
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
# --- For DIAdem-NAVIGATOR ------------------------------------------
dd.AddUserCommandToEvent("dd.Navigator.Events.OnShowingContextMenu","MyNavigatorOnShowingContextMenu")

def MyNavigatorOnShowingContextMenu(ParentObj, MenuPoints):
    MenuPoints.Add("MyMenuPoint1", 1)
    MenuPoints.Add("MyMenuPoint2", 2)
    if not MenuPoints.IsIDUsed(3):
        MenuPoints.Add("MyMenuPoint3",3)

# --- For DIAdem-VIEW ------------------------------------------
dd.AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu","MyViewOnShowingContextMenu")

def MyViewOnShowingContextMenu(Area, MenuPoints):
    MenuPoints.Add("MyMenuPoint1", 1)
    MenuPoints.Add("MyMenuPoint2", 2)
    if not MenuPoints.IsIDUsed(3):
        MenuPoints.Add("MyMenuPoint3",3)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ContextMenu/methods/ContextMenu_method_IsIDUsed_IMenuPoints.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
