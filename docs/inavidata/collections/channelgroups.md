---
title: "ChannelGroups"
description: "Collection of all channel groups of a data set in the script interface for internal data. You use the ChannelGroups collection to access channel groups, to dele"
---

# ChannelGroups

!!! abstract "Collection &middot; `Inavidata.chm`"
    Collection: ChannelGroups <Data>

Collection of all channel groups of a data set in the script interface for internal data. You use the ChannelGroups collection to access channel groups, to delete channel groups, or to add new channel groups. Each element of the ChannelGroups collection is a ChannelGroup .

## Python example

```python
dd.Data.Root.ChannelGroups.RemoveAll()
dd.Data.Root.ChannelGroups.Add("MyChannelGroup")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademchannelgroups-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademchannelgroups-add/">Add</a> | <a href="../../methods/idiademchannelgroups-addchannelgroup/">AddChannelGroup</a> | <a href="../../methods/idiademchannelgroups-exists/">Exists</a> | <a href="../../methods/idiademchannelgroups-item/">Item</a> | <a href="../../methods/idiademchannelgroups-remove/">Remove</a> | <a href="../../methods/idiademchannelgroups-removeall/">RemoveAll</a> | <a href="../../methods/idiademchannelgroups-sort/">Sort</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idiademroot/">Root &lt;Data&gt;</a>.<a href="../../properties/idiademroot-channelgroups/">ChannelGroups</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademChannelGroups.HTM`*
