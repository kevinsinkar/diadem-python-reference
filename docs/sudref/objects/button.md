---
title: "Button"
description: "The Button object corresponds to the Button control in an extended table of a user dialog box. You use the Button object to define a button you want to display "
---

# Button

!!! abstract "Object &middot; `Sudref.chm`"
    Object: Button <XTable>

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

The Button object corresponds to the Button control in an extended table of a user dialog box. You use the Button object to define a button you want to display in an extended table. You use the ButtonShape property to specify whether the button displays as an actual button, or as a toolbar symbol. Note You only can access this control within the event procedures of the extended table.

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr><td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note</strong>  You only can access this control within the event procedures of the extended table.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Cell.ButtonShape = 3  # 0=Standard, 3=Toolbar-Button, 4=Button
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/xtable-alignment/">Alignment</a> | <a href="../../properties/xtable-backcolor/">BackColor</a> | <a href="../../properties/xtable-buttonshape/">ButtonShape</a> | <a href="../../properties/xtable-enable/">Enable</a> | <a href="../../properties/xtable-font/">Font</a> | <a href="../../properties/xtable-forecolor/">ForeColor</a> | <a href="../../properties/xtable-indentation/">Indentation</a> | <a href="../../properties/xtable-interpretedtext/">InterpretedText</a> | <a href="../../properties/xtable-layout/">Layout</a> | <a href="../../properties/xtable-objecttype-2/">ObjectType</a> | <a href="../../properties/xtable-picture/">Picture</a> | <a href="../../properties/xtable-tag-2/">Tag</a> | <a href="../../properties/xtable-text/">Text</a> | <a href="../../properties/xtable-visible/">Visible</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/xtable-refreshtext/">RefreshText</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="../tovirtgridctrl/">XTable</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToBtnRteOb_XTable.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
