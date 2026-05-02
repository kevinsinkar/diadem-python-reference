---
title: "ToSudViewObInt"
description: "The Dialog object provides a non-modal user dialog box, or provides a user dialog box in DIAdem VIEW. Non-modal dialog boxes can remain open while you work with"
---

# ToSudViewObInt

!!! abstract "Object &middot; `Sudref.chm`"
    Object: Dialog <NonModal>

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

The Dialog object provides a non-modal user dialog box, or provides a user dialog box in DIAdem VIEW. Non-modal dialog boxes can remain open while you work with the higher ranking window. You use the Dialog object to define the size of the dialog box and the basic properties of the user dialog box, such as the size, title, and layers.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
MyDlg = SUDDlgCreate("ToolWindow","Example")
iPos = AppRectangleGet(1)  # returns position below the panel bar in pixels
Hor = MyDlg.MapXPixelToDlu(iPos(0)) - MyDlg.Left  # calculates into dialog units
Ver = MyDlg.MapYPixelToDlu(iPos(1)) - MyDlg.Top
MyDlg.Move(Hor, Ver)
MyDlg.Show
```

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "Dialog"
oMyObj.FileName = "Project.sud"
oMyObj.DlgName = "Input"
oMyObj.Dialog.Color = dd.RGB(255, 0, 0)
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/tosudviewobint-borderwidthpix/">BorderWidthPix</a> | <a href="../../properties/tosudviewobint-bottom/">Bottom</a> | <a href="../../properties/tosudviewobint-color/">Color</a> | <a href="../../properties/tosudviewobint-controls/">Controls</a> | <a href="../../properties/tosudviewobint-cursorpointer/">CursorPointer</a> | <a href="../../properties/tosudviewobint-dialogcode/">DialogCode</a> | <a href="../../properties/tosudviewobint-enable/">Enable</a> | <a href="../../properties/tosudviewobint-escapemode/">EscapeMode</a> | <a href="../../properties/tosudviewobint-filename/">FileName</a> | <a href="../../properties/tosudviewobint-filepath/">FilePath</a> | <a href="../../properties/tosudviewobint-font/">Font</a> | <a href="../../properties/tosudviewobint-fontdisp/">FontDisp</a> | <a href="../../properties/tosudviewobint-height/">Height</a> | <a href="../../properties/tosudviewobint-layers/">Layers</a> | <a href="../../properties/tosudviewobint-left/">Left</a> | <a href="../../properties/tosudviewobint-maxscreenheight/">MaxScreenHeight</a> | <a href="../../properties/tosudviewobint-maxscreenwidth/">MaxScreenWidth</a> | <a href="../../properties/tosudviewobint-minheight/">MinHeight</a> | <a href="../../properties/tosudviewobint-minwidth/">MinWidth</a> | <a href="../../properties/tosudviewobint-objectcode/">ObjectCode</a> | <a href="../../properties/tosudviewobint-objecttype/">ObjectType</a> | <a href="../../properties/tosudviewobint-reducedtotitle/">ReducedToTitle</a> | <a href="../../properties/tosudviewobint-right/">Right</a> | <a href="../../properties/tosudviewobint-scrollbars/">ScrollBars</a> | <a href="../../properties/tosudviewobint-scrollheight/">ScrollHeight</a> | <a href="../../properties/tosudviewobint-scrollwidth/">ScrollWidth</a> | <a href="../../properties/tosudviewobint-tag/">Tag</a> | <a href="../../properties/tosudviewobint-title/">Title</a> | <a href="../../properties/tosudviewobint-titleheightpix/">TitleHeightPix</a> | <a href="../../properties/tosudviewobint-tooltiptext/">ToolTipText</a> | <a href="../../properties/tosudviewobint-top/">Top</a> | <a href="../../properties/tosudviewobint-width/">Width</a> | <a href="../../properties/tosudviewobint-writevariables/">WriteVariables</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tosudviewobint-activate/">Activate</a> | <a href="../../methods/tosudviewobint-apply/">Apply</a> | <a href="../../methods/tosudviewobint-beginwaitcursor/">BeginWaitCursor</a> | <a href="../../methods/tosudviewobint-cancel/">Cancel</a> | <a href="../../methods/tosudviewobint-centerwindowoverdiadem/">CenterWindowOverDIAdem</a> | <a href="../../methods/tosudviewobint-endwaitcursor/">EndWaitCursor</a> | <a href="../../methods/tosudviewobint-exporttopicture/">ExportToPicture</a> | <a href="../../methods/tosudviewobint-getcontrol/">GetControl</a> | <a href="../../methods/tosudviewobint-hide/">Hide</a> | <a href="../../methods/tosudviewobint-isvalid/">IsValid</a> | <a href="../../methods/tosudviewobint-mapxdlutopixel/">MapXDluToPixel</a> | <a href="../../methods/tosudviewobint-mapxpixeltodlu/">MapXPixelToDlu</a> | <a href="../../methods/tosudviewobint-mapydlutopixel/">MapYDluToPixel</a> | <a href="../../methods/tosudviewobint-mapypixeltodlu/">MapYPixelToDlu</a> | <a href="../../methods/tosudviewobint-move/">Move</a> | <a href="../../methods/tosudviewobint-ok/">OK</a> | <a href="../../methods/tosudviewobint-refreshall/">RefreshAll</a> | <a href="../../methods/tosudviewobint-restorewaitcursor/">RestoreWaitCursor</a> | <a href="../../methods/tosudviewobint-runclick/">RunClick</a> | <a href="../../methods/tosudviewobint-runcustomaction/">RunCustomAction</a> | <a href="../../methods/tosudviewobint-runcustomactionall/">RunCustomActionAll</a> | <a href="../../methods/tosudviewobint-runinitialize/">RunInitialize</a> | <a href="../../methods/tosudviewobint-runterminate/">RunTerminate</a> | <a href="../../methods/tosudviewobint-setforeground/">SetForeground</a> | <a href="../../methods/tosudviewobint-show/">Show</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToSudViewObInt.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
