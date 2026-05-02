---
title: "EventDragStart.EventDragStart"
description: "Is triggered when you drag a selected element from the tree. The event can only be triggered if dragging is permitted."
---

# EventDragStart.EventDragStart

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventDragStart for Tree

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

Is triggered when you drag a selected element from the tree. The event can only be triggered if dragging is permitted.

## Signature

```python
dd.EventDragOver(ByRef This, ByRef DropInformation, ByRef DropEffect)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventInitialize(This):
    CreateDefaultTree(This)

def Tree1_EventDropAllowed(This, DropInformation, DropEffect):
    if (DropInformation.Text != ""):
        DropEffect = eDropEffectCopy or eDropEffectMove

def Tree1_EventDragStart(This, DropInformation, DropEffect):
    oMySelNode = This.SelectedItem
    oMyDragItem = oMySelNode
    if (not oMySelNode Is None):
        DropInformation.Text = oMySelNode.Text
        DropEffect = eDropEffectCopy or eDropEffectMove

def Tree1_EventDragCompleted(This, DropEffect):
    if (DropEffect == eDropEffectMove):
        if (not oMyDragItem Is None):
            RemoveTreeItem(this, oMyDragItem)

def Tree1_EventDrop(This, DropInformation, DropEffect, Node):
    if (not Node is None):
        if (DropInformation.Text == Node.Text) and (DropEffect == eDropEffectMove):
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
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventDragStart.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
