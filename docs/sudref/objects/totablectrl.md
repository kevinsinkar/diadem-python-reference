---
title: "ToTableCtrl"
description: "The Text object corresponds to the Table control in a user dialog box. You use the Table object to define a table to be displayed in the user dialog box. Use th"
---

# ToTableCtrl

!!! abstract "Object &middot; `Sudref.chm`"
    Object: Table

The Text object corresponds to the Table control in a user dialog box. You use the Table object to define a table to be displayed in the user dialog box. Use the Cells property to specify the table values and use the Columns property to assign table columns to vector variables or matrix variables. Note Use the XTable control to display an extended table. In an extended table you can assign a specific control type to each individual column of the extended table. In the extended table you can display buttons, selection lists, channel selection lists, input fields, texts, or check boxes.

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr><td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note</strong>  Use the <a href="../tovirtgridctrl/">XTable</a> control to display an extended table. In an extended table you can assign a specific control type to each individual column of the extended table. In the extended table you can display buttons, selection lists, channel selection lists, input fields, texts, or check boxes.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Table1.TitleFontColor = vbBlue
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/totablectrl-autoheaderwidth/">AutoHeaderWidth</a> | <a href="../../properties/totablectrl-backcolor/">BackColor</a> | <a href="../../properties/totablectrl-bottom/">Bottom</a> | <a href="../../properties/totablectrl-cells/">Cells</a> | <a href="../../properties/totablectrl-colmoveallowed/">ColMoveAllowed</a> | <a href="../../properties/totablectrl-columns/">Columns</a> | <a href="../../properties/totablectrl-columntitlesdisplay/">ColumnTitlesDisplay</a> | <a href="../../properties/totablectrl-cursorpointer/">CursorPointer</a> | <a href="../../properties/totablectrl-enable/">Enable</a> | <a href="../../properties/totablectrl-font/">Font</a> | <a href="../../properties/totablectrl-forecolor/">ForeColor</a> | <a href="../../properties/totablectrl-headercolor/">HeaderColor</a> | <a href="../../properties/totablectrl-headerwidth/">HeaderWidth</a> | <a href="../../properties/totablectrl-height/">Height</a> | <a href="../../properties/totablectrl-left/">Left</a> | <a href="../../properties/totablectrl-lockupdate/">LockUpdate</a> | <a href="../../properties/totablectrl-objectcode/">ObjectCode</a> | <a href="../../properties/totablectrl-objecttype/">ObjectType</a> | <a href="../../properties/totablectrl-readonly/">ReadOnly</a> | <a href="../../properties/totablectrl-readonlycellcolor/">ReadOnlyCellColor</a> | <a href="../../properties/totablectrl-right/">Right</a> | <a href="../../properties/totablectrl-rowmoveallowed/">RowMoveAllowed</a> | <a href="../../properties/totablectrl-rows/">Rows</a> | <a href="../../properties/totablectrl-rowtitlesdisplay/">RowTitlesDisplay</a> | <a href="../../properties/totablectrl-selcolumn/">SelColumn</a> | <a href="../../properties/totablectrl-selectedcells/">SelectedCells</a> | <a href="../../properties/totablectrl-selrow/">SelRow</a> | <a href="../../properties/totablectrl-tabstop/">TabStop</a> | <a href="../../properties/totablectrl-tag/">Tag</a> | <a href="../../properties/totablectrl-titlefont/">TitleFont</a> | <a href="../../properties/totablectrl-titlefontcolor/">TitleFontColor</a> | <a href="../../properties/totablectrl-tooltiptext/">ToolTipText</a> | <a href="../../properties/totablectrl-top/">Top</a> | <a href="../../properties/totablectrl-transpheaderwidth/">TranspHeaderWidth</a> | <a href="../../properties/totablectrl-verticalorientation/">VerticalOrientation</a> | <a href="../../properties/totablectrl-visible/">Visible</a> | <a href="../../properties/totablectrl-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/totablectrl-layername/">LayerName</a> | <a href="../../methods/totablectrl-move/">Move</a> | <a href="../../methods/totablectrl-refresh/">Refresh</a> | <a href="../../methods/totablectrl-runcustomaction/">RunCustomAction</a> | <a href="../../methods/totablectrl-runinitialize/">RunInitialize</a> | <a href="../../methods/totablectrl-setfocus/">SetFocus</a></p>
</div>
<div class="Events"><h2>Events</h2>
<p><a href="../../events/eventcustomaction-eventcustomaction/">EventCustomAction</a> | <a href="../../events/eventinitialize-eventinitialize/">EventInitialize</a> | <a href="../../events/eventlostfocus-eventlostfocus/">EventLostFocus</a> | <a href="../../events/eventrefresh-eventrefresh/">EventRefresh</a> | <a href="../../events/onitemchange-onitemchange/">OnItemChange</a> | <a href="../../events/onselchange-onselchange/">OnSelChange</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/controls/">Controls</a>.<a href="../../methods/tocmdtarget-item/">Item</a> | <a href="../tosudviewobint/">Dialog &lt;NonModal&gt;</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a> | <a href="../tosudviewobint/">Dialog</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../tocell/">Cell</a> | <a href="../../collections/columns/">Columns</a> | <a href="../../collections/rows/">Rows</a> | <a href="../../collections/selectedcells/">SelectedCells</a> | <a href="#" data-unresolved="1">Object Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToTableCtrl.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
