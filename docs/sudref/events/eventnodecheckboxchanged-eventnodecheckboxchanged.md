---
title: "EventNodeCheckboxChanged.EventNodeCheckboxChanged"
description: "Is triggered in user dialog boxes when the status of the checkbox of a node in the tree changes. Use the Checked property to request or set the status of a node"
---

# EventNodeCheckboxChanged.EventNodeCheckboxChanged

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventNodeCheckboxChanged for Tree

Is triggered in user dialog boxes when the status of the checkbox of a node in the tree changes. Use the Checked property to request or set the status of a node checkbox. DIAdem does not call the EventNodeCheckboxChanged event if you use the Checked property to change the status of a checkbox.

## Signature

```python
dd.EventNodeCheckboxChanged(ByRef This, ByRef Node)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventInitialize(ByRef This):
    CreateDefaultTree(This)

def Tree1_EventNodeCheckboxChanged(ByRef This, ByRef Node):
    sOutput = "Checked nodes:" + VBCrLf
    for oMyNode in This.Nodes:
        if oMyNode.Checked:
            sOutput = sOutput + oMyNode.Text + VBCrLf
        GetCheckedNodes(oMyNode)
    Msgbox(sOutput)

def GetCheckedNodes(oNode):
    for oMyNode in oNode.Nodes:
        if oMyNode.Checked:
            sOutput = sOutput + oMyNode.Text + VBCrLf
        GetCheckedNodes(oMyNode)

def CreateDefaultTree(ByRef This):
    This.Checkboxes = True
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
<div class="SeeAlso">
<h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventNodeCheckboxChanged.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
