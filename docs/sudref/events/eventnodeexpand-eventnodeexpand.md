---
title: "EventNodeExpand.EventNodeExpand"
description: "Is triggered in user dialog boxes when a branch in the tree expands interactively. The Expanded property has the value True when the event occurs. If you set th"
---

# EventNodeExpand.EventNodeExpand

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventNodeExpand for Tree

Is triggered in user dialog boxes when a branch in the tree expands interactively. The Expanded property has the value True when the event occurs. If you set the value of the Expanded property to False , you prevent the branch from expanding. During the initial tree build, DIAdem does not call the event with EventInitialize nor does it call the event when replotting the tree with EventRefresh .

## Signature

```python
dd.EventNodeExpand(ByRef This, ByRef Node)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventInitialize(This):
    CreateDefaultTree(This)

def Tree1_EventNodeExpand(This, Node):
    if Node.Key == "handtool":
        Node.Nodes.RemoveAll
        Node.Nodes.Add("Hammer").Key = "hammer"
        Node.Nodes.Add("Screwdriver").Key = "screwdriver"
        Node.Nodes.Add("Tongs").Key = "tongs"

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
    oMainNode.Nodes.Add("Dummy").Key = "dummy"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventNodeExpand.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
