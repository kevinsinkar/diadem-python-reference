---
title: "ToTabPageCtrl"
description: "The TabPageCtrl object corresponds to the TabPageCtrl control in a user dialog box. You use the TabPageCtrl object to define a series of tabs in a user dialog b"
---

# ToTabPageCtrl

!!! abstract "Object &middot; `Sudref.chm`"
    Object: TabPageCtrl

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

The TabPageCtrl object corresponds to the TabPageCtrl control in a user dialog box. You use the TabPageCtrl object to define a series of tabs in a user dialog box. Each tab can contain any number of controls. This group of controls enables you to clearly display a number of controls in one user dialog box.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyPage = TabPageCtrl1.ActivePage
oMyPage.Title = "Layout"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/totabpagectrl-activepage/">ActivePage</a> | <a href="../../properties/totabpagectrl-activepageindex/">ActivePageIndex</a> | <a href="../../properties/totabpagectrl-activepageindexext/">ActivePageIndexExt</a> | <a href="../../properties/totabpagectrl-bottom/">Bottom</a> | <a href="../../properties/totabpagectrl-cursorpointer/">CursorPointer</a> | <a href="../../properties/totabpagectrl-enable/">Enable</a> | <a href="../../properties/totabpagectrl-font/">Font</a> | <a href="../../properties/totabpagectrl-forecolor/">ForeColor</a> | <a href="../../properties/totabpagectrl-height/">Height</a> | <a href="../../properties/totabpagectrl-left/">Left</a> | <a href="../../properties/totabpagectrl-multiline/">Multiline</a> | <a href="../../properties/totabpagectrl-objectcode/">ObjectCode</a> | <a href="../../properties/totabpagectrl-objecttype/">ObjectType</a> | <a href="../../properties/totabpagectrl-pages/">Pages</a> | <a href="../../properties/totabpagectrl-right/">Right</a> | <a href="../../properties/totabpagectrl-style/">Style</a> | <a href="../../properties/totabpagectrl-tabstop/">TabStop</a> | <a href="../../properties/totabpagectrl-tag/">Tag</a> | <a href="../../properties/totabpagectrl-top/">Top</a> | <a href="../../properties/totabpagectrl-visible/">Visible</a> | <a href="../../properties/totabpagectrl-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/totabpagectrl-layername/">LayerName</a> | <a href="../../methods/totabpagectrl-move/">Move</a> | <a href="../../methods/totabpagectrl-refreshall/">RefreshAll</a> | <a href="../../methods/totabpagectrl-runchange/">RunChange</a> | <a href="../../methods/totabpagectrl-runcustomaction/">RunCustomAction</a> | <a href="../../methods/totabpagectrl-runcustomactionall/">RunCustomActionAll</a> | <a href="../../methods/totabpagectrl-runinitialize/">RunInitialize</a> | <a href="../../methods/totabpagectrl-setfocus/">SetFocus</a></p>
</div>
<div class="Events"><h2>Events</h2>
<p><a href="../../events/tabpagectrl-eventchange/">EventChange</a> | <a href="../../events/eventcustomaction-eventcustomaction/">EventCustomAction</a> | <a href="../../events/tabpagectrl-eventdblclick/">EventDblClick</a> | <a href="../../events/tabpagectrl-eventinitialize/">EventInitialize</a> | <a href="../../events/tabpagectrl-eventmousedown/">EventMouseDown</a> | <a href="../../events/tabpagectrl-eventmousemove/">EventMouseMove</a> | <a href="../../events/tabpagectrl-eventmouseup/">EventMouseUp</a> | <a href="../../events/tabpagectrl-eventrefresh/">EventRefresh</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/controls/">Controls</a>.<a href="../../methods/tocmdtarget-item/">Item</a> | <a href="../tosudviewobint/">Dialog &lt;NonModal&gt;</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a> | <a href="../tosudviewobint/">Dialog</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../collections/pages/">Pages</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToTabPageCtrl.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
