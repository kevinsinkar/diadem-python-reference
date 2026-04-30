---
title: "Channels"
description: "Collection of all channels of a channel group in the script interface for internal data. You use the Channels collection to access channels, to delete channels,"
---

# Channels

!!! abstract "Collection &middot; `Inavidata.chm`"
    Collection: Channels <Data>

Collection of all channels of a channel group in the script interface for internal data. You use the Channels collection to access channels, to delete channels, or to add new channels. Each element of the Channels collection is a Channel .

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.Add("MyChannel",dd.DataTypeFloat64)
for i in range( 1, 100+1):
    oMyChn = []
oMyChn.append(float(i/100000))
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademchannels-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademchannels-add/">Add</a> | <a href="../../methods/idiademchannels-addassignmentchannel/">AddAssignmentChannel</a> | <a href="../../methods/idiademchannels-addcalculationchannel/">AddCalculationChannel</a> | <a href="../../methods/idiademchannels-addcalculationchannelref/">AddCalculationChannelRef</a> | <a href="../../methods/idiademchannels-addchannel/">AddChannel</a> | <a href="../../methods/idiademchannels-addimplicitchannel/">AddImplicitChannel</a> | <a href="../../methods/idiademchannels-addvideochannel/">AddVideoChannel</a> | <a href="../../methods/idiademchannels-exists/">Exists</a> | <a href="../../methods/idiademchannels-getreference/">GetReference</a> | <a href="../../methods/idiademchannels-item/">Item</a> | <a href="../../methods/idiademchannels-remove/">Remove</a> | <a href="../../methods/idiademchannels-removeall/">RemoveAll</a> | <a href="../../methods/idiademchannels-sort/">Sort</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idiademchannelgroup/">ChannelGroup &lt;Data&gt;</a>.<a href="../../properties/idiademchannelgroup-channels/">Channels</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademChannels.HTM`*
