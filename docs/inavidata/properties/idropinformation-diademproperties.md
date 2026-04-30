---
title: "IDropInformation.DiademProperties"
description: "Specifies the properties which drag and drop onto another object. These properties might be DIAdem base properties or custom properties of the channels, the cha"
---

# IDropInformation.DiademProperties

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: DiademProperties for DropInformation

Specifies the properties which drag and drop onto another object. These properties might be DIAdem base properties or custom properties of the channels, the channel groups, or the root. The generated PropertyList collection is read only.

## Signature

```python
return_value = obj.DiademProperties
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_DiademProperties_IDropInformation.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
