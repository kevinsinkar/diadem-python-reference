---
title: "ToGenericOcx"
description: "The ActiveX object provides in a user dialog box an ActiveX control that is already registered on your computer. In addition to the properties and methods the d"
---

# ToGenericOcx

!!! abstract "Object &middot; `Sudref.chm`"
    Object: ActiveX

The ActiveX object provides in a user dialog box an ActiveX control that is already registered on your computer. In addition to the properties and methods the dialog editor provides for the ActiveX control, the ActiveX control has its own properties, events, and methods. You can access the integrated methods and properties of an ActiveX control with the method X via the syntax Object.X.Method or Object.X.Property. Refer to the documentation for the ActiveX controls for detailed descriptions.

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr><td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note</strong>  Use the context menu to add ActiveX controls to the controls bar.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyControl in Dialog.Controls:
    if oMyControl.ObjectType = "ActiveX":
        MsgBoxDisp(oMyControl.ProgID + " / " + oMyControl.ObjectCode)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/togenericocx-backcolor/">BackColor</a> | <a href="../../properties/togenericocx-bottom/">Bottom</a> | <a href="../../properties/togenericocx-cursorpointer/">CursorPointer</a> | <a href="../../properties/togenericocx-enable/">Enable</a> | <a href="../../properties/togenericocx-font/">Font</a> | <a href="../../properties/togenericocx-forecolor/">ForeColor</a> | <a href="../../properties/togenericocx-height/">Height</a> | <a href="../../properties/togenericocx-left/">Left</a> | <a href="../../properties/togenericocx-objectcode/">ObjectCode</a> | <a href="../../properties/togenericocx-objecttype/">ObjectType</a> | <a href="../../properties/togenericocx-progid/">ProgId</a> | <a href="../../properties/togenericocx-right/">Right</a> | <a href="../../properties/togenericocx-tabstop/">TabStop</a> | <a href="../../properties/togenericocx-tag/">Tag</a> | <a href="../../properties/togenericocx-tooltiptext/">ToolTipText</a> | <a href="../../properties/togenericocx-top/">Top</a> | <a href="../../properties/togenericocx-visible/">Visible</a> | <a href="../../properties/togenericocx-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/togenericocx-layername/">LayerName</a> | <a href="../../methods/togenericocx-move/">Move</a> | <a href="../../methods/togenericocx-refresh/">Refresh</a> | <a href="../../methods/togenericocx-runcustomaction/">RunCustomAction</a> | <a href="../../methods/togenericocx-runinitialize/">RunInitialize</a> | <a href="../../methods/togenericocx-setfocus/">SetFocus</a> | <a href="../../methods/togenericocx-x/">X</a></p>
</div>
<div class="Events"><h2>Events</h2>
<p><a href="../../events/eventcustomaction-eventcustomaction/">EventCustomAction</a> | <a href="../../events/eventinitialize-eventinitialize/">EventInitialize</a> | <a href="../../events/eventrefresh-eventrefresh/">EventRefresh</a></p>
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

*Source: `Sudref/objects/SUD_Objects_ToGenericOcx.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
