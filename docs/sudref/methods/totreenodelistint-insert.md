---
title: "ToTreeNodeListInt.Insert"
description: "Adds a new node to a tree in a user dialog box. The new node is created on the level of the TreeNodes object."
---

# ToTreeNodeListInt.Insert

!!! abstract "Method &middot; `Sudref.chm`"
    Method: Insert for TreeNodes

Adds a new node to a tree in a user dialog box. The new node is created on the level of the TreeNodes object.

## Signature

```python
return_value = obj.Insert(Text, Index)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventInitialize(ByRef This):
    CreateDefaultTree(This)

def Button1_EventClick(ByRef This):
    oMyNodes = Tree1.Nodes(1).Nodes
    sNewName = InPutBox("Enter name of new node","New Node")
    oMyNewNode = oMyNodes.Insert(sNewName,1)
    Tree1.Nodes(1).Update(eUpdateModeNodeAndChilds)

def CreateDefaultTree(ByRef This):
    oFindRoot = This.Nodes.Add("Double click any node to add a sub node")
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
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/methods/SUD_method_Insert_ToTreeNodeListInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
