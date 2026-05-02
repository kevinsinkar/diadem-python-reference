---
title: "MenuPoints"
description: "Collection of context menu items."
---

# MenuPoints

!!! abstract "Collection &middot; `ContextMenu.chm`"
    Collection: MenuPoints

Collection of context menu items.

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
    pass
    # select MenuPoint.ID
    # case 1    MsgBoxDisp("DIAdem-NAVIGATOR: MyMenuPoint1 selected")
    # case 2    MsgBoxDisp("DIAdem-NAVIGATOR: MyMenuPoint2 selected")

# --- For DIAdem-VIEW -----------------------------------------------
AddUserCommandToEvent("dd.View.Events.OnShowingContextMenu","MyViewOnShowingContextMenu")
AddUserCommandToEvent("dd.View.Events.OnContextMenuPointSelected","MyViewOnContextMenuPointSelected")

def MyViewOnShowingContextMenu(Area, MenuPoints):
    if (Area.DisplayObjType == "CurveChart2D"):
        MenuPoints.Add("My CurveChart Menu Point", 1)
    if (Area.DisplayObjType == "ChannelTable"):
        MenuPoints.Add("My ChannelTable Menu Point", 2)

def MyViewOnContextMenuPointSelected(Area, MenuPoint):
    pass
    # select MenuPoint.ID
    # case 1    MsgBoxDisp("DIAdem-VIEW: MyMenuPoint1 selected")
    # case 2    MsgBoxDisp("DIAdem-VIEW: MyMenuPoint2 selected")
```

```python
def XTable1_EventContextMenuPointSelected(This, Row, Col, MenuPoint):
    dd.MsgBox("Row: " + Row + "; Column: " + Col + "\r\n" + "Menu entry: " + MenuPoint.Text)

def XTable1_EventContextMenuShowing(This, Row, Col, MenuPoints):
    MenuPoints.Add("Menu 1",1)
    MenuPoints.Add("Menu 2",2)
```

```python
def Tree1_EventInitialize(This):
    CreateDefaultTree(This)

def Tree1_EventContextMenuShowing(This, Node, MenuPoints):
    MenuPoints.Add("Menu 1",1)
    MenuPoints.Add("Menu 2",2)

def Tree1_EventContextMenuPointSelected(This, Node, MenuPoint):
    dd.MsgBox("Selected Node: " + Node.Text + "\r\n" + "Menu entry: " + MenuPoint.Text)

def CreateDefaultTree(This):
    oRoot = This.Nodes.Add("Tools")
    oRoot.Key = "tools"
    oRoot.Expanded = true
    oMainNode = oRoot.Nodes.Add("Electric Tools")
    oMainNode.Key = "electric"
    oMainNode.Nodes.Add("Drill").Key = "drill"
    oMainNode.Nodes.Add("Saw").Key = "saw"
    oMainNode = oRoot.Nodes.Add("Hand Tools")
    oMainNode.Key = "handtool"
    oMainNode.Nodes.Add("Hammer").Key = "hammer"
    oMainNode.Nodes.Add("Screwdriver").Key = "screwdriver"
    oMainNode.Nodes.Add("Tongs").Key = "tongs"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/imenupoints-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/imenupoints-add/">Add</a> | <a href="../../methods/imenupoints-isidused/">IsIDUsed</a> | <a href="../../methods/imenupoints-item/">Item</a> | <a href="../../methods/imenupoints-remove/">Remove</a> | <a href="../../methods/imenupoints-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ContextMenu/objects/ContextMenu_Objects_IMenuPoints.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
