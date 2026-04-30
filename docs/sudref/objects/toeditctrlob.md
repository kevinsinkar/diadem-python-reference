---
title: "ToEditCtrlOb"
description: "The EditBox object corresponds to the EditBox control in a user dialog box. You use the EditBox object to define a textbox that is to be displayed in the dialog"
---

# ToEditCtrlOb

!!! abstract "Object &middot; `Sudref.chm`"
    Object: EditBox

The EditBox object corresponds to the EditBox control in a user dialog box. You use the EditBox object to define a textbox that is to be displayed in the dialog box. You can link the textbox to a SpinBox . You use the Tab Order dialog box to change the order of the SpinBox and the EditBox in the dialog box. If you include a SpinBox in a user dialog box directly after including an EditBox, the two controls are automatically linked. You can then use the SpinBox to edit the numeric value in the EditBox. You can use the EditBuddy property for the SpinBox to disable the link.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
EditBox1.ForeColor = vbBlue
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/toeditctrlob-accelerator/">Accelerator</a> | <a href="../../properties/toeditctrlob-backcolor/">BackColor</a> | <a href="../../properties/toeditctrlob-bottom/">Bottom</a> | <a href="../../properties/toeditctrlob-currentcolumn/">CurrentColumn</a> | <a href="../../properties/toeditctrlob-currentline/">CurrentLine</a> | <a href="../../properties/toeditctrlob-cursorpointer/">CursorPointer</a> | <a href="../../properties/toeditctrlob-enable/">Enable</a> | <a href="../../properties/toeditctrlob-font/">Font</a> | <a href="../../properties/toeditctrlob-forecolor/">ForeColor</a> | <a href="../../properties/toeditctrlob-height/">Height</a> | <a href="../../properties/toeditctrlob-left/">Left</a> | <a href="../../properties/toeditctrlob-objectcode/">ObjectCode</a> | <a href="../../properties/toeditctrlob-objecttype/">ObjectType</a> | <a href="../../properties/toeditctrlob-readonly/">ReadOnly</a> | <a href="../../properties/toeditctrlob-right/">Right</a> | <a href="../../properties/toeditctrlob-tabstop/">TabStop</a> | <a href="../../properties/toeditctrlob-tag/">Tag</a> | <a href="../../properties/toeditctrlob-text/">Text</a> | <a href="../../properties/toeditctrlob-tooltiptext/">ToolTipText</a> | <a href="../../properties/toeditctrlob-top/">Top</a> | <a href="../../properties/toeditctrlob-usecolors/">UseColors</a> | <a href="../../properties/toeditctrlob-visible/">Visible</a> | <a href="../../properties/toeditctrlob-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/toeditctrlob-getselectedtext/">GetSelectedText</a> | <a href="../../methods/toeditctrlob-getselectionbegin/">GetSelectionBegin</a> | <a href="../../methods/toeditctrlob-getselectionend/">GetSelectionEnd</a> | <a href="../../methods/toeditctrlob-layername/">LayerName</a> | <a href="../../methods/toeditctrlob-lines/">Lines</a> | <a href="../../methods/toeditctrlob-move/">Move</a> | <a href="../../methods/toeditctrlob-refresh/">Refresh</a> | <a href="../../methods/toeditctrlob-refreshvalue/">RefreshValue</a> | <a href="../../methods/toeditctrlob-runchange/">RunChange</a> | <a href="../../methods/toeditctrlob-runcustomaction/">RunCustomAction</a> | <a href="../../methods/toeditctrlob-runinitialize/">RunInitialize</a> | <a href="../../methods/toeditctrlob-setfocus/">SetFocus</a></p>
</div>
<div class="Events"><h2>Events</h2>
<p><a href="../../events/eventchange-eventchange/">EventChange</a> | <a href="../../events/eventcustomaction-eventcustomaction/">EventCustomAction</a> | <a href="../../events/eventdblclick-eventdblclick/">EventDblClick</a> | <a href="../../events/eventinitialize-eventinitialize/">EventInitialize</a> | <a href="../../events/eventlostfocus-eventlostfocus/">EventLostFocus</a> | <a href="../../events/eventmousedown-eventmousedown/">EventMouseDown</a> | <a href="../../events/eventmousemove-eventmousemove/">EventMouseMove</a> | <a href="../../events/eventmouseup-eventmouseup/">EventMouseUp</a> | <a href="../../events/eventrefresh-eventrefresh/">EventRefresh</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/controls/">Controls</a>.<a href="../../methods/tocmdtarget-item/">Item</a> | <a href="../tosudviewobint/">Dialog &lt;NonModal&gt;</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a> | <a href="../tosudviewob/">Dialog</a>.<a href="../../methods/tosudviewob-getcontrol/">GetControl</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../collections/lines/">Lines</a> | <a href="../tospinnerrt/">SpinBox</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToEditCtrlOb.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
