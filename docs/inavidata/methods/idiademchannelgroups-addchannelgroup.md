---
title: "IDiademChannelGroups.AddChannelGroup"
description: "Copies a ChannelGroup object in the script interface for internal data and adds the object to the existing ChannelGroup objects."
---

# IDiademChannelGroups.AddChannelGroup

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: AddChannelGroup for ChannelGroups <Data>

Copies a ChannelGroup object in the script interface for internal data and adds the object to the existing ChannelGroup objects.

## Signature

```python
return_value = obj.AddChannelGroup(ChannelGroup, [DestIndex], [UseChnXRelations])
```

## Python example

```python
oMyChnGrp = dd.Data.Root.ActiveChannelGroup
dd.Data.Root.ChannelGroups.AddChannelGroup(oMyChnGrp,2,True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_AddChannelGroup_IDiademChannelGroups.htm`*
