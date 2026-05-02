---
title: "PropertyList"
description: "Collection of the Property <Data> objects which you dragged and dropped onto another object. Use the PropertyList <Data> collection to access an individual prop"
---

# PropertyList

!!! abstract "Collection &middot; `Inavidata.chm`"
    Collection: PropertyList <Data>

Collection of the Property <Data> objects which you dragged and dropped onto another object. Use the PropertyList <Data> collection to access an individual property of the Root , ChannelGroup , or Channel object. These properties might be DIAdem base properties or custom properties of the channels, the channel groups, or the root.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.Events.OnDropPage = "MyOnDropPageEvent"

def MyOnDropPageEvent(Context, DropInformation):
    if DropInformation.IsKindOf(eDropDIAdemElement):
        if False:  # This is a dummy statement for autocompletion
            oMyDropElements = dd.Data.Root.ActiveChannelGroup.Channels(1)
        oMyDropElements = DropInformation.DiademElements
        sOutput = oMyDropElements.Count + " dropped elements:"
        for oMyDropElement in oMyDropElements:
            sOutput = sOutput + "\r\n" + "Name: " + oMyDropElement.Name
    elif DropInformation.IsKindOf(eDropDIAdemProperty):
        if False:  # This is a dummy statement for autocompletion
            oMyDropProperties = dd.Data.Root.ChannelGroups(1).Channels(1).Properties
        oMyDropProperties = DropInformation.DiademProperties
        sOutput = oMyDropProperties.Count + " dropped properties:"
        for oMyDropProperty in oMyDropProperties:
            sOutput = sOutput + "\r\n" + "Name: " + oMyDropProperty.Name + "\t" + "DisplayName: " + oMyDropProperty.DisplayName
    Msgbox(sOutput)
    Context.DoProceed = False
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiadempropertylist-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiadempropertylist-add/">Add</a> | <a href="../../methods/idiadempropertylist-addpropertylist/">AddPropertyList</a> | <a href="../../methods/idiadempropertylist-item/">Item</a> | <a href="../../methods/idiadempropertylist-remove/">Remove</a> | <a href="../../methods/idiadempropertylist-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idropinformation/">DropInformation</a>.<a href="../../properties/idropinformation-diademproperties/">DiademProperties</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademPropertyList.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
