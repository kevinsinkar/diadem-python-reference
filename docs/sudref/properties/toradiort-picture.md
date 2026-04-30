---
title: "ToRadioRt.Picture"
description: "Specifies the graphic for a control in a user dialog box. Click Picture in the Properties tab to paste, to load, or to edit a graphic. You also can specify the "
---

# ToRadioRt.Picture

!!! abstract "Property &middot; `Sudref.chm`"
    Property: Picture for RadioButton

Specifies the graphic for a control in a user dialog box. Click Picture in the Properties tab to paste, to load, or to edit a graphic. You also can specify the color that the transparent control displays. You can embed graphics in a user dialog box or save the link in the file. DIAdem searches for graphic files for user dialogs first in the folder where the SUD file is stored, then in the SCRIPT folders defined in the variables ScriptReadPath and ScriptLibrPath , then in the DIAdem program folder and finally in the media folders. which are defined in the variables MediaReadPath and MediaLibrPath . You can use relative paths and absolute paths. The graphic must be the same size as the graphic specified under PictureOffstate . Under Windows, you can set the screen scaling or DPI value to another value than 100%, such as 150% or 200%. With higher scaling under Windows, graphics in DIAdem dialog boxes might be very small. To display graphics in DIAdem with the screen scaling in the correct size, you can save these graphics in the same folder as the original file, but with the same file name and the postfix _pct150 or _pct200. DIAdem automatically selects the appropriate file depending on the Windows scaling factor. The graphics in these files must be scaled according to the scaling factor set under Windows. For example, if the screen scaling is 150 % and you select the file image.jpg in the Picture Definition dialog box and the same folder also contains the file image_150pct.jpg for a scaling factor of 150%, DIAdem automatically uses the file image_pct150.jpg instead of the initially selected file image.jpg. The picture must not be embedded.

## Signature

```python
obj.Picture
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
RadioButton1.Picture = "\SUD\On.bmp"
RadioButton1.PictureOffState = "\SUD\Off.bmp"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../toradiort-pictureoffstate/">PictureOffstate</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/properties/SUD_property_Picture_ToRadioRt.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
