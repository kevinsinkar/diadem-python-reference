---
title: "ToVarComboRt"
description: "The EnumComboBox object corresponds to the EnumComboBox control in a user dialog box. You use the EnumComboBox object to define a selection list that displays i"
---

# ToVarComboRt

!!! abstract "Object &middot; `Sudref.chm`"
    Object: EnumComboBox

The EnumComboBox object corresponds to the EnumComboBox control in a user dialog box. You use the EnumComboBox object to define a selection list that displays in the user dialog box. The list drops down when you click the box. Specify the displayed selection terms using a dynamic enumeration list variable or an enumeration variable . Note The ComboBox control has similar properties. However, you use ListItems in the Properties tab to specify the selection terms for the control.

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr><td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>The <a href="../tocombort/">ComboBox</a> control has similar properties. However, you use <a href="#" data-unresolved="1">ListItems</a> in the <strong>Properties</strong> tab to specify the selection terms for the control.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
EnumComboBox.Selection = 2
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tovarcombort-accelerator/">Accelerator</a> | <a href="../../properties/tovarcombort-backcolor/">BackColor</a> | <a href="../../properties/tovarcombort-bottom/">Bottom</a> | <a href="../../properties/tovarcombort-combotype/">ComboType</a> | <a href="../../properties/tovarcombort-cursorpointer/">CursorPointer</a> | <a href="../../properties/tovarcombort-enable/">Enable</a> | <a href="../../properties/tovarcombort-font/">Font</a> | <a href="../../properties/tovarcombort-forecolor/">ForeColor</a> | <a href="../../properties/tovarcombort-height/">Height</a> | <a href="../../properties/tovarcombort-left/">Left</a> | <a href="../../properties/tovarcombort-objectcode/">ObjectCode</a> | <a href="../../properties/tovarcombort-objecttype/">ObjectType</a> | <a href="../../properties/tovarcombort-right/">Right</a> | <a href="../../properties/tovarcombort-selection/">Selection</a> | <a href="../../properties/tovarcombort-selectionext/">SelectionExt</a> | <a href="../../properties/tovarcombort-tabstop/">TabStop</a> | <a href="../../properties/tovarcombort-tag/">Tag</a> | <a href="../../properties/tovarcombort-text/">Text</a> | <a href="../../properties/tovarcombort-textext/">TextExt</a> | <a href="../../properties/tovarcombort-tooltiptext/">ToolTipText</a> | <a href="../../properties/tovarcombort-top/">Top</a> | <a href="../../properties/tovarcombort-usecolors/">UseColors</a> | <a href="../../properties/tovarcombort-value/">Value</a> | <a href="../../properties/tovarcombort-valueext/">ValueExt</a> | <a href="../../properties/tovarcombort-visible/">Visible</a> | <a href="../../properties/tovarcombort-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tovarcombort-items/">Items</a> | <a href="../../methods/tovarcombort-layername/">LayerName</a> | <a href="../../methods/tovarcombort-move/">Move</a> | <a href="../../methods/tovarcombort-refresh/">Refresh</a> | <a href="../../methods/tovarcombort-refreshvalue/">RefreshValue</a> | <a href="../../methods/tovarcombort-runchange/">RunChange</a> | <a href="../../methods/tovarcombort-runcustomaction/">RunCustomAction</a> | <a href="../../methods/tovarcombort-runinitialize/">RunInitialize</a> | <a href="../../methods/tovarcombort-setfocus/">SetFocus</a></p>
</div>
<div class="Events"><h2>Events</h2>
<p><a href="../../events/eventchange-eventchange/">EventChange</a> | <a href="../../events/eventcustomaction-eventcustomaction/">EventCustomAction</a> | <a href="../../events/eventinitialize-eventinitialize/">EventInitialize</a> | <a href="../../events/eventlostfocus-eventlostfocus/">EventLostFocus</a> | <a href="../../events/eventmousedown-eventmousedown/">EventMouseDown</a> | <a href="../../events/eventmousemove-eventmousemove/">EventMouseMove</a> | <a href="../../events/eventmouseup-eventmouseup/">EventMouseUp</a> | <a href="../../events/eventrefresh-eventrefresh/">EventRefresh</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/controls/">Controls</a>.<a href="../../methods/tocmdtarget-item/">Item</a> | <a href="../tosudviewobint/">Dialog &lt;NonModal&gt;</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a> | <a href="../tosudviewobint/">Dialog</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../collections/listitems/">ListItems</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToVarComboRt.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
