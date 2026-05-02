---
title: "ToChnListBoxCtrl"
description: "The ChnListBox object corresponds to the ChnListBox control in a user dialog box. You use the ChnListBox object to define a channel selection list to display in"
---

# ToChnListBoxCtrl

!!! abstract "Object &middot; `Sudref.chm`"
    Object: ChnListBox

The ChnListBox object corresponds to the ChnListBox control in a user dialog box. You use the ChnListBox object to define a channel selection list to display in the user dialog box. The user dialog box takes the displayed selection terms from the Data Portal. The channels currently loaded in DIAdem appear in the channel selection list in channel number order. If you drag a channel from the Data Portal to the channel selection list, you select this channel in the channel selection list. If you drag a channel group to the channel selection list, you select the first channel in this channel group. If you drag the data set from the Data Portal to the channel selection list, you select the first channel of the data set. If the property SelectionMode = 1-MultiSelection is set for the channel selection list and you drag several channels from the Data Portal to the channel selection list, the selection list applies the same selection order as the Data Portal. If you drag a channel group to the channel selection list, you select all the channels in this channel group. The same applies if you drag the data set to the channel selection list. The user dialog box determines the contents of the channel selection list when the dialog box opens. Use the Refresh method to update the channel selection list while the dialog box is executed.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
ChnListBox1.Syntax = 5  # channelname only
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tochnlistboxctrl-accelerator/">Accelerator</a> | <a href="../../properties/tochnlistboxctrl-backcolor/">BackColor</a> | <a href="../../properties/tochnlistboxctrl-bottom/">Bottom</a> | <a href="../../properties/tochnlistboxctrl-cursorpointer/">CursorPointer</a> | <a href="../../properties/tochnlistboxctrl-displaynumbers/">DisplayNumbers</a> | <a href="../../properties/tochnlistboxctrl-enable/">Enable</a> | <a href="../../properties/tochnlistboxctrl-font/">Font</a> | <a href="../../properties/tochnlistboxctrl-forecolor/">ForeColor</a> | <a href="../../properties/tochnlistboxctrl-height/">Height</a> | <a href="../../properties/tochnlistboxctrl-left/">Left</a> | <a href="../../properties/tochnlistboxctrl-objectcode/">ObjectCode</a> | <a href="../../properties/tochnlistboxctrl-objecttype/">ObjectType</a> | <a href="../../properties/tochnlistboxctrl-right/">Right</a> | <a href="../../properties/tochnlistboxctrl-selection/">Selection</a> | <a href="../../properties/tochnlistboxctrl-selectionext/">SelectionExt</a> | <a href="../../properties/tochnlistboxctrl-syntax/">Syntax</a> | <a href="../../properties/tochnlistboxctrl-tabstop/">TabStop</a> | <a href="../../properties/tochnlistboxctrl-tag/">Tag</a> | <a href="../../properties/tochnlistboxctrl-text/">Text</a> | <a href="../../properties/tochnlistboxctrl-top/">Top</a> | <a href="../../properties/tochnlistboxctrl-topindex/">TopIndex</a> | <a href="../../properties/tochnlistboxctrl-usecolors/">UseColors</a> | <a href="../../properties/tochnlistboxctrl-value/">Value</a> | <a href="../../properties/tochnlistboxctrl-valueext/">ValueExt</a> | <a href="../../properties/tochnlistboxctrl-visible/">Visible</a> | <a href="../../properties/tochnlistboxctrl-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2><p><a href="../../methods/tochnlistboxctrl-items/">Items</a> | <a href="../../methods/tochnlistboxctrl-layername/">LayerName</a> | <a href="../../methods/tochnlistboxctrl-move/">Move</a> | <a href="../../methods/tochnlistboxctrl-multiselection/">MultiSelection</a> | <a href="../../methods/tochnlistboxctrl-refresh/">Refresh</a> | <a href="../../methods/tochnlistboxctrl-refreshvalue/">RefreshValue</a> | <a href="../../methods/tochnlistboxctrl-runchange/">RunChange</a> | <a href="../../methods/tochnlistboxctrl-runcustomaction/">RunCustomAction</a> | <a href="../../methods/tochnlistboxctrl-runinitialize/">RunInitialize</a> | <a href="../../methods/tochnlistboxctrl-setfocus/">SetFocus</a></p>
</div>
<div class="Events"><h2>Events</h2><p><a href="../../events/eventchange-eventchange/">EventChange</a> | <a href="../../events/eventchnlistrefreshed-eventchnlistrefreshed/">EventChnListRefreshed</a> | <a href="../../events/eventcustomaction-eventcustomaction/">EventCustomAction</a> | <a href="../../events/eventdblclick-eventdblclick/">EventDblClick</a> | <a href="../../events/eventdrop-eventdrop/">EventDrop</a> | <a href="../../events/eventdropallowed-eventdropallowed/">EventDropAllowed</a> | <a href="../../events/eventinitialize-eventinitialize/">EventInitialize</a> | <a href="../../events/eventlostfocus-eventlostfocus/">EventLostFocus</a> | <a href="../../events/eventmousedown-eventmousedown/">EventMouseDown</a> | <a href="../../events/eventmousemove-eventmousemove/">EventMouseMove</a> | <a href="../../events/eventmouseup-eventmouseup/">EventMouseUp</a> | <a href="../../events/eventrefresh-eventrefresh/">EventRefresh</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/controls/">Controls</a>.<a href="../../methods/tocmdtarget-item/">Item</a> | <a href="../tosudviewobint/">Dialog &lt;NonModal&gt;</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a> | <a href="../tosudviewobint/">Dialog</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../collections/chnlistitems/">ListItems</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToChnListBoxCtrl.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
