---
title: "ToTreeNodeInt"
description: "The TreeNode object corresponds to a node in the tree of a user dialog box."
---

# ToTreeNodeInt

!!! abstract "Object &middot; `Sudref.chm`"
    Object: TreeNode

The TreeNode object corresponds to a node in the tree of a user dialog box.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventInitialize(This):
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

def Button1_EventClick(This):
    oMyNode = tree1.SelectedItem
    if (not oMyNode Is None):
        sOutPut = "Node selected: " + oMyNode.Text + "\r\n"
        if oMyNode.Parent is None:
            sOutPut = sOutPut + "Node is root node" + "\r\n"
        else:
            sOutPut = sOutPut + "Parent: " + oMyNode.Parent.Text + "\r\n"
        if oMyNode.PreviousNode is None:
            sOutPut = sOutPut + "Node is first node" + "\r\n"
        else:
            sOutPut = sOutPut + "Previous node: " + oMyNode.PreviousNode.Text + "\r\n"
        if oMyNode.NextNode is None:
            sOutPut = sOutPut + "Node is last node" + "\r\n"
        else:
            sOutPut = sOutPut + "Next node: " + oMyNode.NextNode.Text + "\r\n"
        if oMyNode.Nodes.Count == 0:
            sOutPut = sOutPut + "Node has no children" + "\r\n"
        else:
            sOutPut = sOutPut + "First child: " + oMyNode.Nodes(1).Text + "\r\n"
    else:
        sOutPut = "No node selected."
    dd.MsgBox(sOutPut)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/totreenodeint-backcolor/">BackColor</a> | <a href="../../properties/totreenodeint-bold/">Bold</a> | <a href="../../properties/totreenodeint-checked/">Checked</a> | <a href="../../properties/totreenodeint-expanded/">Expanded</a> | <a href="../../properties/totreenodeint-forecolor/">ForeColor</a> | <a href="../../properties/totreenodeint-index/">Index</a> | <a href="../../properties/totreenodeint-key/">Key</a> | <a href="../../properties/totreenodeint-level/">Level</a> | <a href="../../properties/totreenodeint-nextnode/">NextNode</a> | <a href="../../properties/totreenodeint-nodes/">Nodes</a> | <a href="../../properties/totreenodeint-parent/">Parent</a> | <a href="../../properties/totreenodeint-pictureindex/">PictureIndex</a> | <a href="../../properties/totreenodeint-pictureindexexpanded/">PictureIndexExpanded</a> | <a href="../../properties/totreenodeint-pictureindexselected/">PictureIndexSelected</a> | <a href="../../properties/totreenodeint-previousnode/">PreviousNode</a> | <a href="../../properties/totreenodeint-tag/">Tag</a> | <a href="../../properties/totreenodeint-text/">Text</a> | <a href="../../properties/totreenodeint-tooltiptext/">ToolTipText</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/totreenodeint-update/">Update</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../totreectrl/">Tree</a>.<a href="../../methods/totreectrl-getnode/">GetNode</a> | <a href="../totreectrl/">Tree</a>.<a href="../../properties/totreectrl-selecteditem/">SelectedItem</a> | <a href="./">TreeNode</a>.<a href="../../properties/totreenodeint-nextnode/">NextNode</a> | <a href="./">TreeNode</a>.<a href="../../properties/totreenodeint-parent/">Parent</a> | <a href="./">TreeNode</a>.<a href="../../properties/totreenodeint-previousnode/">PreviousNode</a> | <a href="../../collections/treenodes/">TreeNodes</a>.<a href="../../methods/totreenodelistint-add/">Add</a> | <a href="../../collections/treenodes/">TreeNodes</a>.<a href="../../methods/totreenodelistint-insert/">Insert</a> | <a href="../../collections/treenodes/">TreeNodes</a>.<a href="../../methods/totreenodelistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToTreeNodeInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
