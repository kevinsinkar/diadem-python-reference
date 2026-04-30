---
title: "IToSudDlgInt"
description: "The Dialog object provides access to a user dialog box in DIAdem VIEW. You use the Dialog object to define the size of the dialog box and the basic properties o"
---

# IToSudDlgInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Dialog

The Dialog object provides access to a user dialog box in DIAdem VIEW. You use the Dialog object to define the size of the dialog box and the basic properties of the user dialog box, and also variables and properties. You can design the user dialog box with the dialog editor in DIAdem SCRIPT.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "Dialog"
oMyObj = oMySheet.ActiveArea.DisplayObj
oMyObj.FileName = dd.ProgramDrv + "Libr/Documents/ViewTemplate.sud"
oMyObj.DlgName = "Dlg1"
oMyObj.Dialog.Color = dd.RGB(255, 0, 0)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itosuddlgint-area/">Area</a> | <a href="../../properties/itosuddlgint-dialog/">Dialog</a> | <a href="../../properties/itosuddlgint-dlgname/">DlgName</a> | <a href="../../properties/itosuddlgint-filename/">FileName</a> | <a href="../../properties/itosuddlgint-toolbarvisible/">ToolbarVisible</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itosuddlgint-showdialogdlg/">ShowDialogDlg</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToSudDlgInt.htm`*
