---
title: "IDropInformation.DiademElements"
description: "Specifies the elements from the script interface for internal data which you drag and drop onto another object. These elements can be channels, channel groups, "
---

# IDropInformation.DiademElements

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: DiademElements for DropInformation

Specifies the elements from the script interface for internal data which you drag and drop onto another object. These elements can be channels, channel groups, or the root. The generated ElementList collection is with read only access.

## Signature

```python
return_value = obj.DiademElements
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_DiademElements_IDropInformation.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
