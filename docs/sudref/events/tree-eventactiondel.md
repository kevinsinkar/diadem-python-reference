---
title: "tree.EventActionDel"
description: "Is triggered in user dialog boxes if you press <Del> in the tree."
---

# tree.EventActionDel

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventActionDel for Tree

Is triggered in user dialog boxes if you press <Del> in the tree.

## Signature

```python
dd.EventActionDel(ByRef This)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventActionDel(This):
    if (not Tree1.SelectedItem is None):
        oParentNode = Tree1.SelectedItem.Parent
        if (oParentNode is None):
            Tree1.Nodes.Remove(Tree1.SelectedItem.Key)
            Tree1.Refresh
        else:
            oParentNode.Nodes.Remove(tree1.SelectedItem.Key)
            oParentNode.Update(eUpdateModeNodeAndChilds)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventActionDel_tree.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
