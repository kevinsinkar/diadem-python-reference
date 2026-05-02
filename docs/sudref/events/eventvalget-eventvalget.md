---
title: "EventValGet.EventValGet"
description: "Triggers in user dialog boxes to display the value of a cell of the extended table."
---

# EventValGet.EventValGet

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventValGet for XTable

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

Triggers in user dialog boxes to display the value of a cell of the extended table.

## Signature

```python
dd.EventValGet(ByRef This, Row, Col, ByRef Cell, IsInputCell)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>User the methods <a href="../../methods/tovirtgridctrl-refreshcols/">RefreshCols</a> and <a href="../../methods/tovirtgridctrl-refreshrows/">RefreshRows</a> to refresh single columns or rows of an extended table.</td></tr>
<tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To lock single cells against entries, select entry mode (<span class="Monospace">IsInputCell=TRUE</span>) and set the property <span class="Monospace">Cell</span>.<a href="../../properties/tovirtgridctrl-enable/">Enable</a> = 0.</td></tr>
<tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Do not initialize the control in this event. To configure the control, use the event <a href="../eventcolctrlpreset-eventcolctrlpreset/">EventColCtrlPreset</a> or <a href="../eventdefaultcolctrlpreset-eventdefaultcolctrlpreset/">EventDefaultColCtrlPreset</a> instead.</td></tr>
<tr>
<td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the dialog box <a href="#" data-unresolved="1">Configure columns</a> to determine the type of the control that is assigned to the column with the number <span class="Monospace">Col</span>. To open this dialog box, select the extended table in the dialog editor and click <b>Columns</b> on the <b>Properties</b> tab. You can assign the following types of controls to a column: <a href="../../objects/button/">Button</a>, <a href="../../objects/checkbox/">CheckBox</a>, <a href="../../objects/chncombobox/">ChnComboBox</a>, <a href="../../objects/chnlistbox/">ChnListBox</a>, <a href="../../objects/combobox/">ComboBox</a>, <a href="../../objects/editbox/">EditBox</a>, <a href="../../objects/listbox/">ListBox</a>, and <a href="../../objects/text/">Text</a>. Refer to the the DIAdem Help for information on the properties and methods of these controls. The control properties, which you also can set in the <a href="#" data-unresolved="1">Cell type</a> dialog box of the extended table, are identified accordingly in the DIAdem help.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def XTable1_EventValGet(This, Row, Col, Cell, IsInputCell):
    if Row == 0:
        if Col != 0:
            Cell.Text = dd.Data.Root.ActiveChannelGroup.Channels(Col).Name
        else:
            Cell.Text = ""
    else:
        # select Col
        # case 0
        Cell.Text = Row
        # case else
        if IsInputCell:
            Cell.Text = Str(dd.Data.Root.ActiveChannelGroup.Channels(Col).Values(Row))
        else:
            Cell.Text = Str(dd.Data.Root.ActiveChannelGroup.Channels(Col).Values(Row),"d.d")

def XTable1_EventDefaultColCtrlPreset(Col, Cell, IsInputCell):
    if IsInputCell:
        Cell.ForeColor = dd.RGB(0, 0, 255)
    else:
        Cell.ForeColor = dd.RGB(255, 0, 0)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventValGet.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
