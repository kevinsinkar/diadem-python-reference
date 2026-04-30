---
title: "EventDragCompleted.EventDragCompleted"
description: "Is triggered in user dialog box after a drag process from a tree or within a tree and when the drag process is complete. In this event you can remove, for examp"
---

# EventDragCompleted.EventDragCompleted

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventDragCompleted for Tree

Is triggered in user dialog box after a drag process from a tree or within a tree and when the drag process is complete. In this event you can remove, for example, the dragged node from its original position in tree, if the node was moved. Use the DropEffect parameter to check whether the dropping process was aborted or whether the node was copied or moved. If you do not change the selection in any event while dragging the node, use the SelectedItem property to specify the dragged node. If you do change the selection, you must note the dragged node in a variable in the EventDragStart event.

## Signature

```python
dd.EventDragOver(ByRef This, DropEffect)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventInitialize(ByRef This):
    CreateDefaultTree(This)

def Tree1_EventDropAllowed(ByRef This, DropInformation, ByRef DropEffect):
    if (DropInformation.Text != ""):
        DropEffect = eDropEffectCopy or eDropEffectMove

def Tree1_EventDragStart(ByRef This, ByRef DropInformation, ByRef DropEffect):
    oMySelNode = This.SelectedItem
    oMyDragItem = oMySelNode
    if (not oMySelNode Is None):
        DropInformation.Text = oMySelNode.Text
        DropEffect = eDropEffectCopy or eDropEffectMove

def Tree1_EventDragCompleted(ByRef This, DropEffect):
    if (DropEffect = eDropEffectMove):
        if (not oMyDragItem Is None):
            RemoveTreeItem(this, oMyDragItem)

def Tree1_EventDrop(ByRef This, DropInformation, ByRef DropEffect, ByRef Node):
    if (not Node is None):
        if (DropInformation.Text = Node.Text) and (DropEffect = eDropEffectMove):
            DropEffect = eDropEffectNone
        else:
            oMyNewNode = Node.Nodes.Add(DropInformation.Text)
            Node.Expanded = True
            Node.Update(eUpdateModeNodeAndChilds)
            This.SelectedItem = oMyNewNode
    else:
        oMyNewNode = This.Nodes.Add(DropInformation.Text)
        This.Refresh
        This.SelectedItem = oMyNewNode

def RemoveTreeItem(Tree, Node):
    if (not Node Is None):
        oMyParentNode = Node.Parent
        if (oMyParentNode Is None):
            Tree.Nodes.Remove(Node.Index)
            Tree.Refresh
        else:
            oMyParentNode.Nodes.Remove(Node.Index)
            oMyParentNode.Update(eUpdateModeNodeAndChilds)

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
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventDragCompleted.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
