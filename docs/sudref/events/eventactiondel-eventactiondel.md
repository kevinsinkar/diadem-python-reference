---
title: "EventActionDel.EventActionDel"
description: "Triggers in user dialog boxes when <Del> is pressed in the extended table."
---

# EventActionDel.EventActionDel

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventActionDel for XTable

Triggers in user dialog boxes when <Del> is pressed in the extended table.

## Signature

```python
dd.EventActionDel(ByRef This, ByRef BDone)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The event is not called in the entry mode of a cell. In this case the behavior cannot be modified.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def XTable1_EventActionDel(ByRef This, ByRef bDone):
    if This.SelectedElements.Count = 1:
        oMyChannel = dd.Data.Root.ActiveChannelGroup.Channels(MySel.FirstCol)
        for i in range(MySel.FirstRow, MySel.LastRow + 1):
            oMyChannel.Values(i) = NoValue
        This.Refresh
        BDone = TRUE
    else:
        BDone = FALSE

def XTable1_EventValGet(ByRef This, Row, Col, ByRef Cell, IsInputCell):
    if Row = 0:
        if Col != 0:
            Cell.Text = ChnName(Col)
        else:
            Cell.Text = ""
    else:
        # select Col
        # case 0
        Cell.Text = Row
        # case else
        Cell.Text = Str(dd.Data.Root.ActiveChannelGroup.Channels(Col).Values(Row))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventActionDel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
