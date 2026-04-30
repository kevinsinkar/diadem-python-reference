---
title: "IDiademVideoChannel.ChannelGroup"
description: "Specifies the channel group which contains the specified video channel in the script interface for internal data."
---

# IDiademVideoChannel.ChannelGroup

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: ChannelGroup for VideoChannel <Data>

Specifies the channel group which contains the specified video channel in the script interface for internal data.

## Signature

```python
return_value = obj.ChannelGroup
```

## Python example

```python
oMyVideoChn= dd.Data.Root.ChannelGroups(1).Channels.AddVideoChannel("Video", "Safetytest02.wmv", dd.eFilePathRelative, dd.NoValue, dd.NoValue, 1)
print(oMyVideoChn.ChannelGroup.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_ChannelGroup_IDiademVideoChannel.htm`*
