---
title: "IDiademChannels.AddChannel"
description: "Copies an existing channel in a collection of other channels in the script interface for internal data."
---

# IDiademChannels.AddChannel

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: AddChannel for Channels <Data>

Copies an existing channel in a collection of other channels in the script interface for internal data.

## Signature

```python
return_value = obj.AddChannel(SourceChannel, [DestIndex], [UseChnXRelations])
```

## Python example

```python
oMyChannel = dd.Data.GetChannel("[1]/[2]")
oMyChannelgroup = dd.Data.Root.ChannelGroups(2)
oMyCopyChannel = oMyChannelgroup.Channels.AddChannel(oMyChannel,1,True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_AddChannel_IDiademChannels.htm`*
