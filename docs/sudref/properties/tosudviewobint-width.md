---
title: "ToSudViewObInt.Width"
description: "Specifies the width of a user dialog box. If you assign the Resizeable property to the user dialog box, the property also specifies the minimum size for scalabl"
---

# ToSudViewObInt.Width

!!! abstract "Property &middot; `Sudref.chm`"
    Property: Width for Dialog <NonModal>

Specifies the width of a user dialog box. If you assign the Resizeable property to the user dialog box, the property also specifies the minimum size for scalable user dialog boxes.

## Signature

```python
obj.Width
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>This property does not include the width of the dialog box border, which the <a href="../tosudviewobint-borderwidthpix/">BorderWidthPix</a> property specifies.</td></tr>
<tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  In scripts, you cannot set the <span class="Monospace">Width</span> property less than the minimum width <a href="../tosudviewobint-minwidth/">MinWidth</a>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyDlg = SudDlgCreate("Input","Example.sud")
oMyDlg.Width = 200
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="../tosudviewobint-bottom/">Bottom</a> | <a href="../tosudviewobint-height/">Height</a> | <a href="../tosudviewobint-left/">Left</a> | <a href="../tosudviewobint-right/">Right</a> | <a href="../tosudviewobint-top/">Top</a> | <a href="../../methods/tosudviewobint-mapxdlutopixel/">MapXDluToPixel</a> | <a href="../../methods/tosudviewobint-mapxpixeltodlu/">MapXPixelToDlu</a> | <a href="../tosudviewobint-borderwidthpix/">BorderWidthPix</a> | <a href="../tosudviewobint-titleheightpix/">TitleHeightPix</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/properties/SUD_property_Width_ToSudViewObInt.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
