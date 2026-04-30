---
title: "ToSudViewOb"
description: "The Dialog object corresponds with the user dialog box you edit within the dialog editor. You use the Dialog object to define the size of the dialog box and the"
---

# ToSudViewOb

!!! abstract "Object &middot; `Sudref.chm`"
    Object: Dialog

The Dialog object corresponds with the user dialog box you edit within the dialog editor. You use the Dialog object to define the size of the dialog box and the basic properties of the user dialog box, such as the size, title, and layers.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Button1_EventClick(ByRef This):
    L1 = 200
    Dialog.OK
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tosudviewob-borderwidthpix/">BorderWidthPix</a> | <a href="../../properties/tosudviewob-bottom/">Bottom</a> | <a href="../../properties/tosudviewob-color/">Color</a> | <a href="../../properties/tosudviewob-controls/">Controls</a> | <a href="../../properties/tosudviewob-cursorpointer/">CursorPointer</a> | <a href="../../properties/tosudviewob-dialogcode/">DialogCode</a> | <a href="../../properties/tosudviewob-enable/">Enable</a> | <a href="../../properties/tosudviewob-escapemode/">EscapeMode</a> | <a href="../../properties/tosudviewob-filename/">FileName</a> | <a href="../../properties/tosudviewob-filepath/">FilePath</a> | <a href="../../properties/tosudviewob-font/">Font</a> | <a href="../../properties/tosudviewob-fontdisp/">FontDisp</a> | <a href="../../properties/tosudviewob-height/">Height</a> | <a href="../../properties/tosudviewob-layers/">Layers</a> | <a href="../../properties/tosudviewob-left/">Left</a> | <a href="../../properties/tosudviewob-maxscreenheight/">MaxScreenHeight</a> | <a href="../../properties/tosudviewob-maxscreenwidth/">MaxScreenWidth</a> | <a href="../../properties/tosudviewob-minheight/">MinHeight</a> | <a href="../../properties/tosudviewob-minwidth/">MinWidth</a> | <a href="../../properties/tosudviewob-objectcode/">ObjectCode</a> | <a href="../../properties/tosudviewob-objecttype/">ObjectType</a> | <a href="../../properties/tosudviewob-reducedtotitle/">ReducedToTitle</a> | <a href="../../properties/tosudviewob-right/">Right</a> | <a href="../../properties/tosudviewob-scrollbars/">ScrollBars</a> | <a href="../../properties/tosudviewob-scrollheight/">ScrollHeight</a> | <a href="../../properties/tosudviewob-scrollwidth/">ScrollWidth</a> | <a href="../../properties/tosudviewob-tag/">Tag</a> | <a href="../../properties/tosudviewob-title/">Title</a> | <a href="../../properties/tosudviewob-titleheightpix/">TitleHeightPix</a> | <a href="../../properties/tosudviewob-tooltiptext/">ToolTipText</a> | <a href="../../properties/tosudviewob-top/">Top</a> | <a href="../../properties/tosudviewob-width/">Width</a> | <a href="../../properties/tosudviewob-writevariables/">WriteVariables</a></p>
</div>
<div class="Methods">
<h2>Methods</h2>
<p><a href="../../methods/tosudviewob-apply/">Apply</a> | <a href="../../methods/tosudviewob-beginwaitcursor/">BeginWaitCursor</a> | <a href="../../methods/tosudviewob-cancel/">Cancel</a> | <a href="../../methods/tosudviewob-centerwindowoverdiadem/">CenterWindowOverDIAdem</a> | <a href="../../methods/tosudviewob-endwaitcursor/">EndWaitCursor</a> | <a href="../../methods/tosudviewob-exporttopicture/">ExportToPicture</a> | <a href="../../methods/tosudviewob-getargument/">GetArgument</a> | <a href="../../methods/tosudviewob-getcontrol/">GetControl</a> | <a href="../../methods/tosudviewob-hide/">Hide</a> | <a href="../../methods/tosudviewob-mapxdlutopixel/">MapXDluToPixel</a> | <a href="../../methods/tosudviewob-mapxpixeltodlu/">MapXPixelToDlu</a> | <a href="../../methods/tosudviewob-mapydlutopixel/">MapYDluToPixel</a> | <a href="../../methods/tosudviewob-mapypixeltodlu/">MapYPixelToDlu</a> | <a href="../../methods/tosudviewob-move/">Move</a> | <a href="../../methods/tosudviewob-ok/">OK</a> | <a href="../../methods/tosudviewob-refreshall/">RefreshAll</a> | <a href="../../methods/tosudviewob-restorewaitcursor/">RestoreWaitCursor</a> | <a href="../../methods/tosudviewob-runclick/">RunClick</a> | <a href="../../methods/tosudviewob-runcustomaction/">RunCustomAction</a> | <a href="../../methods/tosudviewob-runcustomactionall/">RunCustomActionAll</a> | <a href="../../methods/tosudviewob-runinitialize/">RunInitialize</a> | <a href="../../methods/tosudviewob-runterminate/">RunTerminate</a> | <a href="../../methods/tosudviewob-setforeground/">SetForeground</a> | <a href="../../methods/tosudviewob-show/">Show</a></p>
</div>
<div class="Events"><h2>Events</h2><p><a href="../../events/eventclick-eventclick/">EventClick</a> | <a href="../../events/eventctrla-eventctrla/">EventCtrlA</a> | <a href="../../events/eventcustomaction-eventcustomaction/">EventCustomAction</a> | <a href="../../events/eventdblclick-eventdblclick/">EventDblClick</a> | <a href="../../events/eventfunckeypressed-eventfunckeypressed/">EventFuncKeyPressed</a> | <a href="../../events/eventinitialize-eventinitialize/">EventInitialize</a> | <a href="../../events/eventinitfinalize-eventinitfinalize/">EventInitFinalize</a> | <a href="../../events/eventmousedown-eventmousedown/">EventMouseDown</a> | <a href="../../events/eventmousemove-eventmousemove/">EventMouseMove</a> | <a href="../../events/eventmouseup-eventmouseup/">EventMouseUp</a> | <a href="../../events/eventqueryclose-eventqueryclose/">EventQueryClose</a> | <a href="../../events/eventterminate-eventterminate/">EventTerminate</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToSudViewOb.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
