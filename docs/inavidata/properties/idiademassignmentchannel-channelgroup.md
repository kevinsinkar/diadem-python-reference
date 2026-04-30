---
title: "IDiademAssignmentChannel.ChannelGroup"
description: "Specifies the channel group, which contains a specific assignment channel, in the script interface for internal data."
---

# IDiademAssignmentChannel.ChannelGroup

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: ChannelGroup for AssignmentChannel <Data>

Specifies the channel group, which contains a specific assignment channel, in the script interface for internal data.

## Signature

```python
return_value = obj.ChannelGroup
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn", "Default Value")
dd.MsgBoxDisp(oMyChn.ChannelGroup.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_ChannelGroup_IDiademAssignmentChannel.htm`*
