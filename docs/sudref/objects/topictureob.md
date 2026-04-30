---
title: "ToPictureOb"
description: "The Picture object corresponds to the Picture control in a user dialog box. You use the Picture object to define a graphic to be displayed in the user dialog bo"
---

# ToPictureOb

!!! abstract "Object &middot; `Sudref.chm`"
    Object: Picture

The Picture object corresponds to the Picture control in a user dialog box. You use the Picture object to define a graphic to be displayed in the user dialog box. You can load a graphic, insert a graphic from the clipboard, or create a new graphic. Note Use the Layout property to specify the size and the position of the graphic.

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr><td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note</strong>  Use the <a href="../../properties/topictureob-layout/">Layout</a> property to specify the size and the position of the graphic.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Picture1.Picture = "\SUD\Pict1.bmp"
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2><p><a href="../../properties/topictureob-bottom/">Bottom</a> | <a href="../../properties/topictureob-cursorpointer/">CursorPointer</a> | <a href="../../properties/topictureob-enable/">Enable</a> | <a href="../../properties/topictureob-height/">Height</a> | <a href="../../properties/topictureob-layout/">Layout</a> | <a href="../../properties/topictureob-left/">Left</a> | <a href="../../properties/topictureob-objectcode/">ObjectCode</a> | <a href="../../properties/topictureob-objecttype/">ObjectType</a> | <a href="../../properties/topictureob-picture/">Picture</a> | <a href="../../properties/topictureob-right/">Right</a> | <a href="../../properties/topictureob-rotateangle/">RotateAngle</a> | <a href="../../properties/topictureob-tag/">Tag</a> | <a href="../../properties/topictureob-tooltiptext/">ToolTipText</a> | <a href="../../properties/topictureob-top/">Top</a> | <a href="../../properties/topictureob-transparentcolor/">TransparentColor</a> | <a href="../../properties/topictureob-visible/">Visible</a> | <a href="../../properties/topictureob-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/topictureob-layername/">LayerName</a> | <a href="../../methods/topictureob-move/">Move</a> | <a href="../../methods/topictureob-refresh/">Refresh</a> | <a href="../../methods/topictureob-runclick/">RunClick</a> | <a href="../../methods/topictureob-runcustomaction/">RunCustomAction</a> | <a href="../../methods/topictureob-runinitialize/">RunInitialize</a></p>
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

*Source: `Sudref/objects/SUD_Objects_ToPictureOb.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
