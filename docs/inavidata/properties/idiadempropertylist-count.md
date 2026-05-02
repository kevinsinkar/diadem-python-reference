---
title: "IDiademPropertyList.Count"
description: "Specifies the number of properties which you dragged and dropped onto another object. These properties might be DIAdem base properties or custom properties of t"
---

# IDiademPropertyList.Count

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Count for PropertyList <Data>

Specifies the number of properties which you dragged and dropped onto another object. These properties might be DIAdem base properties or custom properties of the channels, the channel groups, or the root.

## Signature

```python
obj.Count
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.Events.OnDropPage = "MyOnDropPageEvent"

def MyOnDropPageEvent(Context, DropContext):
    if DropContext.IsKindOf(eDropDIAdemElement):
        if False:  # This is a dummy statement for autocompletion
            oMyDropElements = dd.Data.Root.ActiveChannelGroup.Channels(1)
        oMyDropElements = DropContext.DiademElements
        sOutput = oMyDropElements.Count + " dropped elements:"
        for oMyDropElement in oMyDropElements:
            sOutput = sOutput + "\r\n" + "Name: " + oMyDropElement.Name
    elif DropContext.IsKindOf(eDropDIAdemProperty):
        if False:  # This is a dummy statement for autocompletion
            oMyDropProperties = dd.Data.Root.ChannelGroups(1).Channels(1).Properties
        oMyDropProperties = DropContext.DiademProperties
        sOutput = oMyDropProperties.Count + " dropped properties:"
        for oMyDropProperty in oMyDropProperties:
            sOutput = sOutput + "\r\n" + "Name: " + oMyDropProperty.Name + "\t" + "DisplayName: " + oMyDropProperty.DisplayName
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

*Source: `Inavidata/properties/DiaCmpnt_property_Count_IDiademPropertyList.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
