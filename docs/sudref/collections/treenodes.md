---
title: "TreeNodes"
description: "Collection of all Nodes in a branch of a tree in a user dialog box."
---

# TreeNodes

!!! abstract "Collection &middot; `Sudref.chm`"
    Collection: TreeNodes

Collection of all Nodes in a branch of a tree in a user dialog box.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventInitialize(ByRef This):
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

def Button1_EventClick(ByRef This):
    oMyNode = tree1.SelectedItem
    if (not oMyNode Is None):
        sOutPut = "Node selected: " + oMyNode.Text + VBCrLf
        if oMyNode.Parent is None:
            sOutPut = sOutPut + "Node is root node" + VBCrLf
        else:
            sOutPut = sOutPut + "Parent: " + oMyNode.Parent.Text + VBCrLf
        if oMyNode.PreviousNode is None:
            sOutPut = sOutPut + "Node is first node" + VBCrLf
        else:
            sOutPut = sOutPut + "Previous node: " + oMyNode.PreviousNode.Text + VBCrLf
        if oMyNode.NextNode is None:
            sOutPut = sOutPut + "Node is last node" + VBCrLf
        else:
            sOutPut = sOutPut + "Next node: " + oMyNode.NextNode.Text + VBCrLf
        if oMyNode.Nodes.Count = 0:
            sOutPut = sOutPut + "Node has no children" + VBCrLf
        else:
            sOutPut = sOutPut + "First child: " + oMyNode.Nodes(1).Text + VBCrLf
    else:
        sOutPut = "No node selected."
    dd.MsgBox(sOutPut)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/totreenodelistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/totreenodelistint-add/">Add</a> | <a href="../../methods/totreenodelistint-insert/">Insert</a> | <a href="../../methods/totreenodelistint-item/">Item</a> | <a href="../../methods/totreenodelistint-remove/">Remove</a> | <a href="../../methods/totreenodelistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/totreectrl/">Tree</a>.<a href="../../properties/totreectrl-nodes/">Nodes</a> | <a href="../../objects/totreenodeint/">TreeNode</a>.<a href="../../properties/totreenodeint-nodes/">Nodes</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToTreeNodeListInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
