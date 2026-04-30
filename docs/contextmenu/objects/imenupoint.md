---
title: "IMenuPoint"
description: "The MenuPoint object provides an item in the context menu."
---

# IMenuPoint

!!! abstract "Object &middot; `ContextMenu.chm`"
    Object: MenuPoint

The MenuPoint object provides an item in the context menu.

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
AddUserCommandToEvent("dd.Navigator.Events.OnContextMenuPointSelected","MyNavigatorOnContextMenuPointSelected")

def MyNavigatorOnShowingContextMenu(ParentObj, MenuPoints):
    if (ParentObj.IsKindOf("Browser")):
        MenuPoints.Add("My Browser Menu Point", 1)
    if (ParentObj.IsKindOf("ResultsList")):
        MenuPoints.Add("My ResultsList Menu Point", 2)

def MyNavigatorOnContextMenuPointSelected(ParentObj, MenuPoint):
    # select MenuPoint.ID
    # case 1    MsgBoxDisp("DIAdem-NAVIGATOR: MyMenuPoint1 selected")
    # case 2    MsgBoxDisp("DIAdem-NAVIGATOR: MyMenuPoint2 selected")

# --- For DIAdem-VIEW -----------------------------------------------
AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu","MyViewOnShowingContextMenu")
AddUserCommandToEvent("dd.View.Events.OnContextMenuPointSelected","MyViewOnContextMenuPointSelected")

def MyViewOnShowingContextMenu(Area, MenuPoints):
    if (Area.DisplayObjType = "CurveChart2D"):
        MenuPoints.Add("My CurveChart Menu Point", 1)
    if (Area.DisplayObjType = "ChannelTable"):
        MenuPoints.Add("My ChannelTable Menu Point", 2)

def MyViewOnContextMenuPointSelected(Area, MenuPoint):
    # select MenuPoint.ID
    # case 1    MsgBoxDisp("DIAdem-VIEW: MyMenuPoint1 selected")
    # case 2    MsgBoxDisp("DIAdem-VIEW: MyMenuPoint2 selected")
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p class="Body"><a href="../../properties/imenupoint-check/">Check</a> | <a href="../../properties/imenupoint-enable/">Enable</a> | <a href="../../properties/imenupoint-id/">ID</a> | <a href="../../properties/imenupoint-menupoints/">MenuPoints</a> | <a href="../../properties/imenupoint-tag/">Tag</a> | <a href="../../properties/imenupoint-text/">Text</a></p>
</div>
<div class="ReturnFrom">
<h2>Returned From</h2>
<p><a href="../../collections/menupoints/">MenuPoints</a>.<a href="../../methods/imenupoints-add/">Add</a> | <a href="../../collections/menupoints/">MenuPoints</a>.<a href="../../methods/imenupoints-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ContextMenu/objects/ContextMenu_Objects_IMenuPoint.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
