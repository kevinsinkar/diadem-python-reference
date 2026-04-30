---
title: "EventSelChanged.EventSelChanged"
description: "Triggers in user dialog boxes if the selection in the extended table changes."
---

# EventSelChanged.EventSelChanged

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventSelChanged for XTable

Triggers in user dialog boxes if the selection in the extended table changes.

## Signature

```python
dd.EventSelChanged(ByRef This)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The properties <span class="Monospace">ActiveCellCol</span> and <span class="Monospace">ActiveCellRow</span> do not contain the current values in the <span class="Monospace">EventSelChanged</span> event if you select the cells with the mouse. Use the <a href="../eventactivecellmoved-eventactivecellmoved/">EventActiveCellMoved</a> event if you want to respond when the enabled cell changes.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def XTable1_EventSelChanged(ByRef This):
    for i in range(1, This.SelectedElements.Count + 1):
        N = This.SelectedElements(i).LastRow - This.SelectedElements(i).FirstRow + 1
        MsgBoxDisp(i + ", Number: " + N)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventSelChanged.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
