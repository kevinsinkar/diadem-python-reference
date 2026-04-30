---
title: "EventDefaultColCtrlPreset.EventDefaultColCtrlPreSet"
description: "Triggers when the user dialog box opens or when the RunDefaultColCtrlPreSet method is used in the user dialog box. You can use this event to configure the contr"
---

# EventDefaultColCtrlPreset.EventDefaultColCtrlPreSet

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventDefaultColCtrlPreSet for XTable

Triggers when the user dialog box opens or when the RunDefaultColCtrlPreSet method is used in the user dialog box. You can use this event to configure the controls that are assigned to the columns of an extended table and that are <Default> type. Use the EventColCtrlPreset event to configure the controls that are not <Default> type.

## Signature

```python
dd.EventDefaultColCtrlPreSet(ByRef This, ByRef Cell, IsInputCell)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>This event triggers twice: once for the control of the display mode and once for the control of the entry mode.</td></tr>
<tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the dialog box <a href="#" data-unresolved="1">Configure columns</a> to determine the type of the &lt;Default&gt; control. To open this dialog box, select the extended table in the dialog editor and click <b>Columns</b> on the <b>Properties</b> tab. You can assign the following types of controls to a column: <a href="../../objects/button/">Button</a>, <a href="../../objects/checkbox/">CheckBox</a>, <a href="../../objects/chncombobox/">ChnComboBox</a>, <a href="../../objects/chnlistbox/">ChnListBox</a>, <a href="../../objects/combobox/">ComboBox</a>, <a href="../../objects/editbox/">EditBox</a>, <a href="../../objects/listbox/">ListBox</a>, and <a href="../../objects/text/">Text</a>. Refer to the the DIAdem Help for information on the properties and methods of these controls. The control properties, which you also can set in the <a href="#" data-unresolved="1">Cell type</a> dialog box of the extended table, are identified accordingly in the DIAdem help.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def XTable1_EventDefaultColCtrlPreSet(ByRef This, ByRef Cell, IsInputCell):
    Cell.Items.RemoveAll
    Cell.FillItemsByVar("ColorLst",True)
    if IsInputCell:
        Cell.BackColor = RGB(255, 0, 0)
    else:
        Cell.BackColor = RGB(0, 0, 255)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventDefaultColCtrlPreset.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
