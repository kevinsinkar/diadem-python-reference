---
title: "IDropInformation.IsKindOf"
description: "Checks whether a DropInformation object is a certain type."
---

# IDropInformation.IsKindOf

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: IsKindOf for DropInformation

Checks whether a DropInformation object is a certain type.

## Signature

```python
bIsKindOf = Object.IsKindOf(sObjectType)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.Events.Drop.OnPage = "MyOnDropPageEvent"

def MyOnDropPageEvent(Context, DropInformation):
    if DropInformation.IsKindOf(eDropDIAdemElement):
        oMyDropElements = DropInformation.DiademElements
        sOutput = oMyDropElements.Count + " dropped elements:"
        for oMyDropElement in oMyDropElements:
            if oMyDropElement.IsKindOf(eDataRoot):
                sOutput = sOutput + "\r\n" + "Root name:" + "\t" + oMyDropElement.Name
            elif oMyDropElement.IsKindOf(eDataChannelGroup):
                sOutput = sOutput + "\r\n" + "Group name:" + "\t" + oMyDropElement.Name
            elif oMyDropElement.IsKindOf(eDataChannel):
                sOutput = sOutput + "\r\n" + "Channel name:" + "\t" + oMyDropElement.Name
    elif DropInformation.IsKindOf(eDropDIAdemProperty):
        oMyDropProperties = DropInformation.DiademProperties
        sOutput = oMyDropProperties.Count + " dropped properties:"
        for oMyDropProperty in oMyDropProperties:
            if oMyDropProperty.Element.IsKindOf(eDataRoot):
                sOutput = sOutput + "\r\n" + "Root property:" + "\t" + oMyDropProperty.Name + "\t" + "; DisplayName: " + oMyDropProperty.DisplayName
            elif oMyDropProperty.Element.IsKindOf(eDataChannelGroup):
                sOutput = sOutput + "\r\n" + "Group property:" + "\t" + oMyDropProperty.Name + "\t" + "; DisplayName: " + oMyDropProperty.DisplayName
            elif oMyDropProperty.Element.IsKindOf(eDataChannel):
                sOutput = sOutput + "\r\n" + "Channel property:" + "\t" + oMyDropProperty.Name + "\t" + "; DisplayName: " + oMyDropProperty.DisplayName
    Msgbox(sOutput)
    Context.DoProceed = False
```

```python
def XTable1_EventDrop(This, Row, Col, DropInformation):
    if DropInformation.IsKindOf(eDropText):
        Msgbox(DropInformation.Text)
    elif DropInformation.IsKindOf(eDropDataStoreElement):
        Msgbox(DropInformation.DataStoreElements.Count)

def XTable1_EventValGet(This, Row, Col, Cell, IsInputCell):
    Cell.Text = ""

def XTable1_EventDropAllowed(This, Row, Col, DropInformation, DropEffect):
    DropEffect = eDropEffectCopy
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_IsKindOf_IDropInformation.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
