---
title: "ToTreeCtrl"
description: "The Tree object corresponds to the Tree control in a user dialog box. Use the Tree object to define a tree to be displayed in the dialog box. Create the tree co"
---

# ToTreeCtrl

!!! abstract "Object &middot; `Sudref.chm`"
    Object: Tree

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

The Tree object corresponds to the Tree control in a user dialog box. Use the Tree object to define a tree to be displayed in the dialog box. Create the tree contents in the script. Create the content in the EventInitialize event and change it dynamically in a different event.

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
    oMainNode.Nodes.Add("Dummy").Key = "dummy"

def Tree1_EventNodeExpand(This, Node):
    if Node.Key == "handtool":
        Node.Nodes.RemoveAll
        Node.Nodes.Add("Hammer").Key = "hammer"
        Node.Nodes.Add("Screwdriver").Key = "screwdriver"
        Node.Nodes.Add("Tongs").Key = "tongs"

def Tree1_EventNodeClick(This, Node):
    dd.MsgBox(Node.Text + " clicked")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/totreectrl-backcolor/">BackColor</a> | <a href="../../properties/totreectrl-borderstyle/">BorderStyle</a> | <a href="../../properties/totreectrl-bottom/">Bottom</a> | <a href="../../properties/totreectrl-checkboxes/">Checkboxes</a> | <a href="../../properties/totreectrl-cursorpointer/">CursorPointer</a> | <a href="../../properties/totreectrl-dragallowed/">DragAllowed</a> | <a href="../../properties/totreectrl-enable/">Enable</a> | <a href="../../properties/totreectrl-font/">Font</a> | <a href="../../properties/totreectrl-forecolor/">ForeColor</a> | <a href="../../properties/totreectrl-height/">Height</a> | <a href="../../properties/totreectrl-hideselection/">HideSelection</a> | <a href="../../properties/totreectrl-left/">Left</a> | <a href="../../properties/totreectrl-nodes/">Nodes</a> | <a href="../../properties/totreectrl-objectcode/">ObjectCode</a> | <a href="../../properties/totreectrl-objecttype/">ObjectType</a> | <a href="../../properties/totreectrl-readonly/">ReadOnly</a> | <a href="../../properties/totreectrl-right/">Right</a> | <a href="../../properties/totreectrl-selecteditem/">SelectedItem</a> | <a href="../../properties/totreectrl-tabstop/">TabStop</a> | <a href="../../properties/totreectrl-tag/">Tag</a> | <a href="../../properties/totreectrl-top/">Top</a> | <a href="../../properties/totreectrl-visible/">Visible</a> | <a href="../../properties/totreectrl-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/totreectrl-getnode/">GetNode</a> | <a href="../../methods/totreectrl-layername/">LayerName</a> | <a href="../../methods/totreectrl-move/">Move</a> | <a href="../../methods/totreectrl-refresh/">Refresh</a> | <a href="../../methods/totreectrl-runcustomaction/">RunCustomAction</a> | <a href="../../methods/totreectrl-runinitialize/">RunInitialize</a> | <a href="../../methods/totreectrl-scrollnodeinview/">ScrollNodeInView</a> | <a href="../../methods/totreectrl-setfocus/">SetFocus</a></p>
</div>
<div class="Events"><h2>Events</h2>
<p><a href="../../events/eventafterlabeledit-eventafterlabeledit/">EventAfterLabelEdit</a> | <a href="../../events/eventbeforelabeledit-eventbeforelabeledit/">EventBeforeLabelEdit</a> | <a href="../../events/tree-eventcontextmenupointselected/">EventContextMenuPointSelected</a> | <a href="../../events/tree-eventcontextmenushowing/">EventContextMenuShowing</a> | <a href="../../events/eventcustomaction-eventcustomaction/">EventCustomAction</a> | <a href="../../events/eventdragcompleted-eventdragcompleted/">EventDragCompleted</a> | <a href="../../events/eventdragover-eventdragover/">EventDragOver</a> | <a href="../../events/eventdragstart-eventdragstart/">EventDragStart</a> | <a href="../../events/eventdrop-eventdrop/">EventDrop</a> | <a href="../../events/eventdropallowed-eventdropallowed/">EventDropAllowed</a> | <a href="../../events/eventinitialize-eventinitialize/">EventInitialize</a> | <a href="../../events/eventlostfocus-eventlostfocus/">EventLostFocus</a> | <a href="../../events/eventnodecheckboxchanged-eventnodecheckboxchanged/">EventNodeCheckboxChanged</a> | <a href="../../events/eventnodeclick-eventnodeclick/">EventNodeClick</a> | <a href="../../events/eventnodecollapse-eventnodecollapse/">EventNodeCollapse</a> | <a href="../../events/eventnodedblclick-eventnodedblclick/">EventNodeDblClick</a> | <a href="../../events/eventnodeexpand-eventnodeexpand/">EventNodeExpand</a> | <a href="../../events/eventrefresh-eventrefresh/">EventRefresh</a> | <a href="../../events/eventselecteditemchanged-eventselecteditemchanged/">EventSelectedItemChanged</a></p>
</div>
<div class="ReturnFrom">
<h2>Returned From</h2>
<p><a href="../../collections/controls/">Controls</a>.<a href="../../methods/tocmdtarget-item/">Item</a> | <a href="../tosudviewobint/">Dialog &lt;NonModal&gt;</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a> | <a href="../tosudviewob/">Dialog</a>.<a href="../../methods/tosudviewob-getcontrol/">GetControl</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Events</h2>
<p><a href="../../events/eventafterlabeledit-eventafterlabeledit/">EventAfterLabelEdit</a> | <a href="../../events/eventbeforelabeledit-eventbeforelabeledit/">EventBeforeLabelEdit</a> | <a href="../../events/tree-eventcontextmenupointselected/">EventContextMenuPointSelected</a> | <a href="../../events/tree-eventcontextmenushowing/">EventContextMenuShowing</a> | <a href="../../events/eventdragover-eventdragover/">EventDragOver</a> | <a href="../../events/eventdropallowed-eventdropallowed/">EventDropAllowed</a> | <a href="../../events/eventnodecheckboxchanged-eventnodecheckboxchanged/">EventNodeCheckboxChanged</a> | <a href="../../events/eventnodeclick-eventnodeclick/">EventNodeClick</a> | <a href="../../events/eventnodedblclick-eventnodedblclick/">EventNodeDblClick</a> | <a href="../../events/eventnodecollapse-eventnodecollapse/">EventNodeCollapse</a> | <a href="../../events/eventnodeexpand-eventnodeexpand/">EventNodeExpand</a> | <a href="../../events/eventselecteditemchanged-eventselecteditemchanged/">EventSelectedItemChanged</a> </p>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToTreeCtrl.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
