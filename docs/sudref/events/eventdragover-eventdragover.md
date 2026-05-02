---
title: "EventDragOver.EventDragOver"
description: "Is triggered in user dialog boxes during a drag process onto a tree. The event can only be triggered if the EventDropAllowed event permits dropping. The event i"
---

# EventDragOver.EventDragOver

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventDragOver for Tree

Is triggered in user dialog boxes during a drag process onto a tree. The event can only be triggered if the EventDropAllowed event permits dropping. The event is triggered as long as the cursor idles over the control. You specify whether a drop process is possible with the DropEffect parameter. For example, it might depend on the node over which the cursor is. If you want to use the entire area of the Tree object as a drop target and if the drop process is independent of specific nodes, use the EventDropAllowed event and evaluate the DropInformation object.

## Signature

```python
dd.EventDragOver(ByRef This, DropInformation, ByRef DropEffect, ByRef Node)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventInitialize(This):
    CreateDefaultTree(This)

def Tree1_EventDropAllowed(This, DropInformation, DropEffect):
    DropEffect = eDropEffectCopy

def Tree1_EventDragOver(This, DropInformation, DropEffect, Node):
    if Node is None:
        DropEffect = eDropEffectNone
    elif Node.Level == 2:
        DropEffect = eDropEffectCopy
    else:
        DropEffect = eDropEffectNone

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventDragOver.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
