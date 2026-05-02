---
title: "EventDrop.EventDrop"
description: "Is triggered when you drag and drop an element from the Data Portal to a channel selection list. The event can only be triggered if Dropping is permitted. The e"
---

# EventDrop.EventDrop

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventDrop

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

Is triggered when you drag and drop an element from the Data Portal to a channel selection list. The event can only be triggered if Dropping is permitted. The event is triggered if the cursor is above the channel selection list and you release the left mouse button.

## Signature

```python
dd.EventDrop(ByRef This, DropInformation, ByRef DoProceed)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ChnListBox1_EventDropAllowed(This, DropInformation, DropEffect):
    oMyElem = DropInformation.DiademElements
    DropEffect = eDropEffectNone
    if oMyElem.Count > 0:
        if oMyElem(1).IsKindOf(eDataChannel):
            if oMyElem(1).DataType == DataTypeFloat64:
                DropEffect = eDropEffectCopy

def ChnListBox1_EventDrop(This, DropInformation, DoProceed):
    MsgBoxDisp(DropInformation.DiademElements(1).Name + " / " + DropInformation.DiademElements(1).Size)
    # further instructions
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventDrop.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
