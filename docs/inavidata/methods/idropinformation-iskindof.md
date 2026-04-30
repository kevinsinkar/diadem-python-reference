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
                sOutput = sOutput + VBCrLf + "Root name:" + VBTab + oMyDropElement.Name
                ElseIf oMyDropElement.IsKindOf(eDataChannelGroup) :
                sOutput = sOutput + VBCrLf + "Group name:" + VBTab + oMyDropElement.Name
                ElseIf oMyDropElement.IsKindOf(eDataChannel) :
                sOutput = sOutput + VBCrLf + "Channel name:" + VBTab + oMyDropElement.Name
        ElseIf  DropInformation.IsKindOf(eDropDIAdemProperty) :
        oMyDropProperties = DropInformation.DiademProperties
        sOutput = oMyDropProperties.Count + " dropped properties:"
        for oMyDropProperty in oMyDropProperties:
            if oMyDropProperty.Element.IsKindOf(eDataRoot):
                sOutput = sOutput + VBCrLf + "Root property:" + VBTab + oMyDropProperty.Name + VBTab + "; DisplayName: " + oMyDropProperty.DisplayName
                ElseIf oMyDropProperty.Element.IsKindOf(eDataChannelGroup) :
                sOutput = sOutput + VBCrLf + "Group property:" + VBTab + oMyDropProperty.Name + VBTab + "; DisplayName: " + oMyDropProperty.DisplayName
                ElseIf oMyDropProperty.Element.IsKindOf(eDataChannel) :
                sOutput = sOutput + VBCrLf + "Channel property:" + VBTab + oMyDropProperty.Name + VBTab + "; DisplayName: " + oMyDropProperty.DisplayName
    Msgbox(sOutput)
    Context.DoProceed = False
```

```python
def XTable1_EventDrop(ByRef This, Row, Col, DropInformation):
    if DropInformation.IsKindOf(eDropText):
        Msgbox(DropInformation.Text)
        ElseIf DropInformation.IsKindOf(eDropDataStoreElement) :
        Msgbox(DropInformation.DataStoreElements.Count)

def XTable1_EventValGet(ByRef This, Row, Col, ByRef Cell, IsInputCell):
    Cell.Text = ""

def XTable1_EventDropAllowed(ByRef This, Row, Col, DropInformation, ByRef DropEffect):
    DropEffect = eDropEffectCopy
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_IsKindOf_IDropInformation.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
