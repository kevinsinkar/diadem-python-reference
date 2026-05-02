---
title: "EventDropAllowed.EventDropAllowed"
description: "Is triggered in user dialog boxes when an element is dragged and dropped onto a channel selection list or an entry field. The event is triggered when you move t"
---

# EventDropAllowed.EventDropAllowed

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventDropAllowed

Is triggered in user dialog boxes when an element is dragged and dropped onto a channel selection list or an entry field. The event is triggered when you move the cursor into the control. Use this event to determine whether dropping onto the control is allowed.

## Signature

```python
dd.EventDropAllowed(ByRef This, DropInformation, ByRef DropEffect)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ChnComboBox1_EventDropAllowed(This, DropInformation, DropEffect):
    oMyElem = DropInformation.DiademElements
    DropEffect = eDropEffectNone
    if oMyElem.Count > 0:
        if oMyElem(1).IsKindOf(eDataChannel):
            if oMyElem(1).DataType == DataTypeFloat64:
                DropEffect = eDropEffectCopy

def ChnComboBox1_EventDrop(This, DropInformation, DoProceed):
    MsgBoxDisp(DropInformation.DiademElements(1).Name + " / " + DropInformation.DiademElements(1).Size)
    # further instructions
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventDropAllowed.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
