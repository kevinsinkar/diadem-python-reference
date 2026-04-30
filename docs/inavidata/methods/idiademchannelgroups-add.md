---
title: "IDiademChannelGroups.Add"
description: "Creates a new channel group in the script interface for internal data and adds the channel group to the ChannelGroups collection. The Add method returns a Chann"
---

# IDiademChannelGroups.Add

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Add for ChannelGroups <Data>

Creates a new channel group in the script interface for internal data and adds the channel group to the ChannelGroups collection. The Add method returns a ChannelGroup object.

## Signature

```python
return_value = obj.Add(Name, [DestIndex])
```

## Python example

```python
dd.Data.Root.ChannelGroups.RemoveAll()
dd.Data.Root.ChannelGroups.Add("MyChnGroup")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Add_IDiademChannelGroups.HTM`*
