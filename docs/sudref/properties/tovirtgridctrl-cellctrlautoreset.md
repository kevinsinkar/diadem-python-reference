---
title: "ToVirtGridCtrl.CellCtrlAutoReset"
description: "Specifies in user dialog boxes whether the extended table automatically resets the control, which is assigned to a cell, to its default settings, after the cell"
---

# ToVirtGridCtrl.CellCtrlAutoReset

!!! abstract "Property &middot; `Sudref.chm`"
    Property: CellCtrlAutoReset for XTable

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

Specifies in user dialog boxes whether the extended table automatically resets the control, which is assigned to a cell, to its default settings, after the cell is displayed. The default settings are the settings that you define for the control in the dialog editor. If you also use the events EventDefaultColCtrlPreset or EventColCtrlPreset to initialize a control, the settings are also included when the control is reset. The default value for this property is 1.

## Signature

```python
obj.CellCtrlAutoReset
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  To display the extended table faster, disable automatic resetting. To do this, assign the value 0-No to the <span class="Monospace">CellCtrlAutoReset</span> property. You must then keep to the following procedures in the script.<p class="Body">In AutoReset mode, the <span class="Monospace">EventValGet</span> event enters the text <span class="Monospace">Test</span> in all cells of the first table row. The remaining table cells do not contain any text.</p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p></div>
<div class="codeblue">
<pre><donottranslate><span class="HlVBSKeyword">Sub</span> XTable1_EventValGet(<span class="HlVBSKeyword">ByRef</span> This, Row, Col, <span class="HlVBSKeyword">ByRef</span> Cell, IsInputCell)
  <span class="HlVBSKeyword">If</span> Row = <span class="HlNumbers">1</span> <span class="HlVBSKeyword">Then</span>
    Cell.Text = <span class="HlString">"Test"</span> 
  <span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">If</span>
<span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">Sub</span></donottranslate></pre>
</div>
<p class="Body">If you disable the AutoReset mode by setting <span class="Monospace">This.CellCtrlAutoReset=0</span> in the <span class="Monospace">EventInitialize</span> event of the extended table, notice that all the table cells contain the text <span class="Monospace">Test</span>. When you disable this mode, the properties of the control are no longer reset. Because the control is used to display all the cells to which the control is assigned, the text <span class="Monospace">Test</span> appears in each of these table cells. When you disable the AutoReset mode, you must therefore extend the script as follows.</p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p></div>
<div class="codeblue">
<pre><donottranslate><span class="HlVBSKeyword">Sub</span> XTable1_EventvalGet(<span class="HlVBSKeyword">ByRef</span> This, Row, Col, <span class="HlVBSKeyword">ByRef</span> Cell, IsInputCell)
  <span class="HlVBSKeyword">If</span> Row = <span class="HlNumbers">1</span> <span class="HlVBSKeyword">Then</span>
    Cell.Text = <span class="HlString">"Test"</span> 
  <span class="HlVBSKeyword">Else</span>
    Cell.Text = <span class="HlString">""</span>
  <span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">If</span>
<span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">Sub</span></donottranslate></pre>
</div>
</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Always ensure that each table cell property that you set in a specific case is reset in all other cases.</td></tr>
<tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>An extended table consists of the controls that you assign to the individual columns and the <span class="Monospace">Text</span> control for the table labels. You must adhere to the above procedures for each control.</td></tr>
<tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The extended table displays much faster if you use controls that contain extensive data and that must refresh repeatedly, such as ListBoxes with many entries.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def XTable1_EventValGet(This, Row, Col, Cell, IsInputCell):
    if Row == 1:
        Cell.Text = "Test"
```

```python
def XTable1_EventvalGet(This, Row, Col, Cell, IsInputCell):
    if Row == 1:
        Cell.Text = "Test"
    else:
        Cell.Text = ""
```

```python
def XTable1_EventInitialize(This):
    This.CellCtrlAutoReset = 0
def XTable1_EventValGet(This, Row, Col, Cell, IsInputCell):
    if Row == 1:
        Cell.Text = "Test"
    else:
        Cell.Text = ""
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/properties/SUD_property_CellCtrlAutoReset_ToVirtGridCtrl.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
