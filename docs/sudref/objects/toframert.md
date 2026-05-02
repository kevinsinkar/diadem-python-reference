---
title: "ToFrameRt"
description: "The Frame object corresponds to the Frame control in a user dialog box. You use the Frame object to define a frame to be displayed in the user dialog box. The f"
---

# ToFrameRt

!!! abstract "Object &middot; `Sudref.chm`"
    Object: Frame

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

The Frame object corresponds to the Frame control in a user dialog box. You use the Frame object to define a frame to be displayed in the user dialog box. The frame does not affect the properties of the grouped controls.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Frame1.Text = "Paramaters"
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2><p><a href="../../properties/toframert-alignment/">Alignment</a> | <a href="../../properties/toframert-backcolor/">BackColor</a> | <a href="../../properties/toframert-bordercolor/">BorderColor</a> | <a href="../../properties/toframert-borderstyle/">BorderStyle</a> | <a href="../../properties/toframert-borderwidth/">BorderWidth</a> | <a href="../../properties/toframert-bottom/">Bottom</a> | <a href="../../properties/toframert-cursorpointer/">CursorPointer</a> | <a href="../../properties/toframert-enable/">Enable</a> | <a href="../../properties/toframert-font/">Font</a> | <a href="../../properties/toframert-forecolor/">ForeColor</a> | <a href="../../properties/toframert-height/">Height</a> | <a href="../../properties/toframert-highlightcolor/">HighlightColor</a> | <a href="../../properties/toframert-interpretedtext/">InterpretedText</a> | <a href="../../properties/toframert-left/">Left</a> | <a href="../../properties/toframert-objectcode/">ObjectCode</a> | <a href="../../properties/toframert-objecttype/">ObjectType</a> | <a href="../../properties/toframert-right/">Right</a> | <a href="../../properties/toframert-tag/">Tag</a> | <a href="../../properties/toframert-text/">Text</a> | <a href="../../properties/toframert-tooltiptext/">ToolTipText</a> | <a href="../../properties/toframert-top/">Top</a> | <a href="../../properties/toframert-visible/">Visible</a> | <a href="../../properties/toframert-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2><p><a href="../../methods/toframert-layername/">LayerName</a> | <a href="../../methods/toframert-move/">Move</a> | <a href="../../methods/toframert-refresh/">Refresh</a> | <a href="../../methods/toframert-refreshtext/">RefreshText</a> | <a href="../../methods/toframert-refreshvalue/">RefreshValue</a> | <a href="../../methods/toframert-runcustomaction/">RunCustomAction</a> | <a href="../../methods/toframert-runinitialize/">RunInitialize</a></p>
</div>
<div class="Events"><h2>Events</h2>
<p><a href="../../events/eventclick-eventclick/">EventClick</a> | <a href="../../events/eventcustomaction-eventcustomaction/">EventCustomAction</a> | <a href="../../events/eventdblclick-eventdblclick/">EventDblClick</a> | <a href="../../events/eventinitialize-eventinitialize/">EventInitialize</a> | <a href="../../events/eventmousedown-eventmousedown/">EventMouseDown</a> | <a href="../../events/eventmousemove-eventmousemove/">EventMouseMove</a> | <a href="../../events/eventmouseup-eventmouseup/">EventMouseUp</a> | <a href="../../events/eventrefresh-eventrefresh/">EventRefresh</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/controls/">Controls</a>.<a href="../../methods/tocmdtarget-item/">Item</a> | <a href="../tosudviewobint/">Dialog &lt;NonModal&gt;</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a> | <a href="../tosudviewobint/">Dialog</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToFrameRt.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
