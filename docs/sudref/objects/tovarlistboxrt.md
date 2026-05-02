---
title: "ToVarListBoxRt"
description: "The EnumListBox object corresponds to the EnumListBox control in a user dialog box. You use the EnumListBox object to define a selection list to be displayed in"
---

# ToVarListBoxRt

!!! abstract "Object &middot; `Sudref.chm`"
    Object: EnumListBox

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

The EnumListBox object corresponds to the EnumListBox control in a user dialog box. You use the EnumListBox object to define a selection list to be displayed in the user dialog box. Specify the displayed selection terms using a dynamic enumeration list variable or an enumeration variable . Note The ListBox control has similar properties. However, you use ListItems in the Properties tab to specify the selection terms for the control.

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr><td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>The <a href="../tolistboxrt/">ListBox</a> control has similar properties. However, you use <a href="#" data-unresolved="1">ListItems</a> in the <strong>Properties</strong> tab to specify the selection terms for the control.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
EnumListBox1.Selection = 2
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tovarlistboxrt-accelerator/">Accelerator</a> | <a href="../../properties/tovarlistboxrt-backcolor/">BackColor</a> | <a href="../../properties/tovarlistboxrt-bottom/">Bottom</a> | <a href="../../properties/tovarlistboxrt-cursorpointer/">CursorPointer</a> | <a href="../../properties/tovarlistboxrt-enable/">Enable</a> | <a href="../../properties/tovarlistboxrt-font/">Font</a> | <a href="../../properties/tovarlistboxrt-forecolor/">ForeColor</a> | <a href="../../properties/tovarlistboxrt-height/">Height</a> | <a href="../../properties/tovarlistboxrt-left/">Left</a> | <a href="../../properties/tovarlistboxrt-objectcode/">ObjectCode</a> | <a href="../../properties/tovarlistboxrt-objecttype/">ObjectType</a> | <a href="../../properties/tovarlistboxrt-right/">Right</a> | <a href="../../properties/tovarlistboxrt-selection/">Selection</a> | <a href="../../properties/tovarlistboxrt-selectionext/">SelectionExt</a> | <a href="../../properties/tovarlistboxrt-tabstop/">TabStop</a> | <a href="../../properties/tovarlistboxrt-tag/">Tag</a> | <a href="../../properties/tovarlistboxrt-text/">Text</a> | <a href="../../properties/tovarlistboxrt-textext/">TextExt</a> | <a href="../../properties/tovarlistboxrt-tooltiptext/">ToolTipText</a> | <a href="../../properties/tovarlistboxrt-top/">Top</a> | <a href="../../properties/tovarlistboxrt-usecolors/">UseColors</a> | <a href="../../properties/tovarlistboxrt-value/">Value</a> | <a href="../../properties/tovarlistboxrt-valueext/">ValueExt</a> | <a href="../../properties/tovarlistboxrt-visible/">Visible</a> | <a href="../../properties/tovarlistboxrt-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tovarlistboxrt-items/">Items</a> | <a href="../../methods/tovarlistboxrt-layername/">LayerName</a> | <a href="../../methods/tovarlistboxrt-move/">Move</a> | <a href="../../methods/tovarlistboxrt-refresh/">Refresh</a> | <a href="../../methods/tovarlistboxrt-refreshvalue/">RefreshValue</a> | <a href="../../methods/tovarlistboxrt-runchange/">RunChange</a> | <a href="../../methods/tovarlistboxrt-runcustomaction/">RunCustomAction</a> | <a href="../../methods/tovarlistboxrt-runinitialize/">RunInitialize</a> | <a href="../../methods/tovarlistboxrt-setfocus/">SetFocus</a></p>
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

*Source: `Sudref/objects/SUD_Objects_ToVarListBoxRt.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
