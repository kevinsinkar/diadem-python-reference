---
title: "Tree.EventContextMenuShowing"
description: "Is triggered in user dialog boxes by a right-click before the context menu displays. If you use the event EventContextMenuShowing , DIAdem no longer requests th"
---

# Tree.EventContextMenuShowing

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventContextMenuShowing for Tree

Is triggered in user dialog boxes by a right-click before the context menu displays. If you use the event EventContextMenuShowing , DIAdem no longer requests the EventNodeClick when you right-click.

## Signature

```python
dd.EventContextMenuShowing(ByRef This, ByRef Node, MenuPoints)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventInitialize(ByRef This):
    CreateDefaultTree(This)

def Tree1_EventContextMenuShowing(ByRef This, ByRef Node, MenuPoints):
    MenuPoints.Add("Menu 1",1)
    MenuPoints.Add("Menu 2",2)

def Tree1_EventContextMenuPointSelected(ByRef This, ByRef Node, MenuPoint):
    dd.MsgBox("Selected Node: " + Node.Text + VBCrLf + "Menu entry: " + MenuPoint.Text)

def CreateDefaultTree(ByRef This):
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventContextMenuShowing_Tree.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
