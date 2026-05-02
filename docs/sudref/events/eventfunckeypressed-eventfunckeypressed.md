---
title: "EventFuncKeyPressed.EventFuncKeyPressed"
description: "Triggers in user dialog boxes when a function key is pressed. You can use this event anywhere, for any purpose."
---

# EventFuncKeyPressed.EventFuncKeyPressed

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventFuncKeyPressed for Dialog

Triggers in user dialog boxes when a function key is pressed. You can use this event anywhere, for any purpose.

## Signature

```python
dd.EventFuncKeyPressed(ByRef This, KeyName, Ctrl, Shift, ByRef DoProceed)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Dialog_EventFuncKeyPressed(This, KeyName, Ctrl, Shift, DoProceed):
    # select KeyName
    # case "F1"
    MsgBoxDisp("F1 pressed")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventFuncKeyPressed.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
