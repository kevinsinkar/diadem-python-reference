---
title: "ToTaskPanelCtrl"
description: "The TaskPanel object corresponds to the TaskPanel control in a user dialog box. Use the TaskPanel object to define a control with expandable groups containing s"
---

# ToTaskPanelCtrl

!!! abstract "Object &middot; `Sudref.chm`"
    Object: TaskPanel

The TaskPanel object corresponds to the TaskPanel control in a user dialog box. Use the TaskPanel object to define a control with expandable groups containing sub-entries in the dialog box. Create the control contents in the script. Create the content in the EventInitialize event and change it dynamically in a different event. Use the SelectedItem property to specify the selected entry and to react to a click on this entry in the EventChange event.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def TaskPanel1_EventInitialize(ByRef This):
    CreateDefaultTaskPanel(This)

def CreateDefaultTaskPanel(ByRef This):
    This.AddGroup("electricGroup", "Electric Tools")
    This.AddGroup("handtoolGroup", "Hand Tools")
    This.AddGroup("textonlyGroup", "Info")
    This.AddLinkItem("electricGroup","drill","Drill")
    This.AddLinkItem("electricGroup","saw","Saw")
    This.AddLinkItem("handtoolGroup","hammer","Hammer")
    This.AddLinkItem("handtoolGroup","screwdriver","Screwdriver")
    This.AddLinkItem("handtoolGroup","tongs","Tongs")
    This.AddTextItem("textonlyGroup","version","Version 1.0")

def TaskPanel1_EventChange(ByRef This):
    TabPageCtrl1.ActivePageIndex = This.SelectedItem
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/totaskpanelctrl-bottom/">Bottom</a> | <a href="../../properties/totaskpanelctrl-enable/">Enable</a> | <a href="../../properties/totaskpanelctrl-height/">Height</a> | <a href="../../properties/totaskpanelctrl-left/">Left</a> | <a href="../../properties/totaskpanelctrl-objectcode/">ObjectCode</a> | <a href="../../properties/totaskpanelctrl-objecttype/">ObjectType</a> | <a href="../../properties/totaskpanelctrl-right/">Right</a> | <a href="../../properties/totaskpanelctrl-selecteditem/">SelectedItem</a> | <a href="../../properties/totaskpanelctrl-tabstop/">TabStop</a> | <a href="../../properties/totaskpanelctrl-tag/">Tag</a> | <a href="../../properties/totaskpanelctrl-top/">Top</a> | <a href="../../properties/totaskpanelctrl-visible/">Visible</a> | <a href="../../properties/totaskpanelctrl-width/">Width</a></p>
</div>
<div class="Methods">
<h2>Methods</h2>
<p><a href="../../methods/totaskpanelctrl-addgroup/">AddGroup</a> | <a href="../../methods/totaskpanelctrl-addlinkitem/">AddLinkItem</a> | <a href="../../methods/totaskpanelctrl-addtextitem/">AddTextItem</a> | <a href="../../methods/totaskpanelctrl-collapsegroup/">CollapseGroup</a> | <a href="../../methods/totaskpanelctrl-expandgroup/">ExpandGroup</a> | <a href="../../methods/totaskpanelctrl-iskindof/">IsKindOf</a> | <a href="../../methods/totaskpanelctrl-itemexists/">ItemExists</a> | <a href="../../methods/totaskpanelctrl-layername/">LayerName</a> | <a href="../../methods/totaskpanelctrl-move/">Move</a> | <a href="../../methods/totaskpanelctrl-refresh/">Refresh</a> | <a href="../../methods/totaskpanelctrl-removeitem/">RemoveItem</a> | <a href="../../methods/totaskpanelctrl-removeitems/">RemoveItems</a> | <a href="../../methods/totaskpanelctrl-runchange/">RunChange</a> | <a href="../../methods/totaskpanelctrl-runcustomaction/">RunCustomAction</a> | <a href="../../methods/totaskpanelctrl-runinitialize/">RunInitialize</a> | <a href="../../methods/totaskpanelctrl-setfocus/">SetFocus</a> | <a href="../../methods/totaskpanelctrl-setitemtext/">SetItemText</a> | <a href="../../methods/totaskpanelctrl-setpictureindex/">SetPictureIndex</a></p>
</div>
<div class="Events"><h2>Events</h2><p><a href="../../events/eventchange-eventchange/">EventChange</a> | <a href="../../events/eventcustomaction-eventcustomaction/">EventCustomAction</a> | <a href="../../events/eventinitialize-eventinitialize/">EventInitialize</a> | <a href="../../events/eventlostfocus-eventlostfocus/">EventLostFocus</a> | <a href="../../events/eventrefresh-eventrefresh/">EventRefresh</a></p></div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/controls/">Controls</a>.<a href="../../methods/tocmdtarget-item/">Item</a> | <a href="../tosudviewobint/">Dialog &lt;NonModal&gt;</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a> | <a href="../tosudviewob/">Dialog</a>.<a href="../../methods/tosudviewob-getcontrol/">GetControl</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToTaskPanelCtrl.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
