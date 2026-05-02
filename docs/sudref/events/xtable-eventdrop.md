---
title: "XTable.EventDrop"
description: "Is triggered when you drag and drop an element from the Data Portal onto a channel selection list. The event can only be triggered if Dropping is permitted."
---

# XTable.EventDrop

!!! abstract "Event &middot; `Sudref.chm`"
    Event: EventDrop for XTable

Is triggered when you drag and drop an element from the Data Portal onto a channel selection list. The event can only be triggered if Dropping is permitted.

## Signature

```python
dd.EventDrop(ByRef This, Row, Col, DropInformation)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyCalc = CalculationSet.CalculationGroups(1).Calculations(1)

def XTable1_EventInitialize(This):
    This.RowCount = oMyCalc.Inputs.Count
    This.Columns.Count = 2

def XTable1_EventValGet(This, Row, Col, Cell, IsInputCell):
    if Row == 0:
        pass
        # select Col
        # case 0    Cell.Text = ""
        # case 1    Cell.Text = "DataType"
        # case 2    Cell.Text = "Reference"
else:
    # select Col
    # case 0    Cell.Text = Str(Row)
    # case 1    Select Case oMyCalc.Inputs(Row).ReferenceType
    # case eReferenceTypeChannel
    Cell.Text = "Channel"
    # case eReferenceTypeChannelList
    Cell.Text = "Channel list"
# case 2    Select Case oMyCalc.Inputs(Row).ReferenceType
# case eReferenceTypeChannel
Cell.Text = oMyCalc.Inputs(Row).Reference.Channel
# case eReferenceTypeChannelList
Cell.Text = oMyCalc.Inputs(Row).Reference.ChannelList

def XTable1_EventDropAllowed(This, Row, Col, DropInformation, DropEffect):
    DropEffect = eDropEffectNone
    if (Row > 0) and (Col == 2):
        oMyElem = DropInformation.DiademElements
        if (oMyElem.Count > 0):
            if oMyElem(1).IsKindOf(eDataChannel):
                DropEffect = eDropEffectCopy
            elif oMyElem(1).IsKindOf(eDataChannelGroup) and (oMyCalc.Inputs(Row).ReferenceType == eReferenceTypeChannelList):
                DropEffect = eDropEffectCopy

def XTable1_EventDrop(This, Row, Col, DropInformation):
    if (Row > 0) and (Col == 2):
        oMyElem = DropInformation.DiademElements
        # select oMyCalc.Inputs(Row).ReferenceType
        # case eReferenceTypeChannel
        oMyCalc.Inputs(Row).Reference.Channel = oMyElem(1).GetReference(eRefTypeIndexName)
        # case eReferenceTypeChannelList
        if oMyElem(1).IsKindOf(eDataChannelGroup):
            oMyCalc.Inputs(Row).Reference.ChannelList = oMyElem(1).Channels.GetReference(eRefTypeIndexName)
        else:
            oMyCalc.Inputs(Row).Reference.ChannelList = oMyElem.GetReference(eRefTypeIndexName)
    This.RefreshRows(Row, Row)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><p class="body"><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Opening the Dialog Editor</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p>
</div>
</div>

---

*Source: `Sudref/events/sud_event_EventDrop_XTable.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
