---
title: "Selection"
description: "Collection of all Selections of an extended table in a user dialog box. A selection consists of several adjacent, selected table cells. You can use the Selectio"
---

# Selection

!!! abstract "Collection &middot; `Sudref.chm`"
    Collection: Selection

Collection of all Selections of an extended table in a user dialog box. A selection consists of several adjacent, selected table cells. You can use the Selection collection to delete selections in the extended table or to extend existing selections. Use the Selection Properties dialog box to specify the selection options in an extended table. To open this dialog box, select the extended table in the dialog editor and click Selection on the Properties tab.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
if XTable1.SelectedElements.Count > 0:
    if XTable1.SelectedElements(1).IsTable:
        MsgBoxDisp ("Entire table selected")
    for i in range(1, XTable1.SelectedElements.Count + 1):
        if XTable1.SelectedElements(i).IsRows:
            lNumRow = XTable1.SelectedElements(i).LastRow - XTable1.SelectedElements(i).FirstRow + 1
            MsgBoxDisp (i + ", NumRow:"& lNumRow)
            ElseIf XTable1.SelectedElements(i).IsCols :
            lNumCol = XTable1.SelectedElements(i).LastCol - XTable1.SelectedElements(i).FirstCol + 1
            MsgBoxDisp (i + ", NumCol:"& lNumCol)
            ElseIf XTable1.SelectedElements(i).IsCells :
            lNumCol = XTable1.SelectedElements(i).LastCol - XTable1.SelectedElements(i).FirstCol + 1
            MsgBoxDisp (i + ", NumCol:"& lNumCol)
            lNumRow = XTable1.SelectedElements(i).LastRow - XTable1.SelectedElements(i).FirstRow + 1
            MsgBoxDisp (i + ", NumRow:"& lNumRow)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tovirtselectionint-allowcells/">AllowCells</a> | <a href="../../properties/tovirtselectionint-allowcols/">AllowCols</a> | <a href="../../properties/tovirtselectionint-allowrows/">AllowRows</a> | <a href="../../properties/tovirtselectionint-allowtable/">AllowTable</a> | <a href="../../properties/tovirtselectionint-blockmode/">BlockMode</a> | <a href="../../properties/tovirtselectionint-colormode/">ColorMode</a> | <a href="../../properties/tovirtselectionint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tovirtselectionint-addcells/">AddCells</a> | <a href="../../methods/tovirtselectionint-addcols/">AddCols</a> | <a href="../../methods/tovirtselectionint-addrows/">AddRows</a> | <a href="../../methods/tovirtselectionint-item/">Item</a> | <a href="../../methods/tovirtselectionint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/tovirtgridctrl/">XTable</a>.<a href="../../properties/tovirtgridctrl-selectedelements/">SelectedElements</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToVirtSelectionInt.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
