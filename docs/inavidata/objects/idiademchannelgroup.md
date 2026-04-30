---
title: "IDiademChannelGroup"
description: "The ChannelGroup object provides a channel group and the associated channels and Properties in the script interface for internal data. The ChannelGroup object i"
---

# IDiademChannelGroup

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: ChannelGroup <Data>

The ChannelGroup object provides a channel group and the associated channels and Properties in the script interface for internal data. The ChannelGroup object is an element of the ChannelGroups collection.

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups.Add("MyChannelGroup")
oMyChn = oMyGrp.Channels.Add("MyChannel",dd.DataTypeFloat64)
for i in range( 1, 100+1):
    oMyChn.Values[i] = float(i/100000)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademchannelgroup-channels/">Channels</a> | <a href="../../properties/idiademchannelgroup-isactive/">IsActive</a> | <a href="../../properties/idiademchannelgroup-name/">Name</a> | <a href="../../properties/idiademchannelgroup-properties/">Properties</a> | <a href="../../properties/idiademchannelgroup-root/">Root</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademchannelgroup-activate/">Activate</a> | <a href="../../methods/idiademchannelgroup-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idiademassignmentchannel/">AssignmentChannel &lt;Data&gt;</a>.<a href="../../properties/idiademassignmentchannel-channelgroup/">ChannelGroup</a> | <a href="../idiademcalculationchannel/">CalculationChannel &lt;Data&gt;</a>.<a href="../../properties/idiademcalculationchannel-channelgroup/">ChannelGroup</a> | <a href="../idiademchannel/">Channel &lt;Data&gt;</a>.<a href="../../properties/idiademchannel-channelgroup/">ChannelGroup</a> | <a href="../../collections/channelgroups/">ChannelGroups &lt;Data&gt;</a>.<a href="../../methods/idiademchannelgroups-add/">Add</a> | <a href="../../collections/channelgroups/">ChannelGroups &lt;Data&gt;</a>.<a href="../../methods/idiademchannelgroups-addchannelgroup/">AddChannelGroup</a> | <a href="../../collections/channelgroups/">ChannelGroups &lt;Data&gt;</a>.<a href="../../methods/idiademchannelgroups-item/">Item</a> | <a href="../idiademcomplexchannel/">ComplexChannel &lt;Data&gt;</a>.<a href="../../properties/idiademcomplexchannel-channelgroup/">ChannelGroup</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-add/">Add</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-item/">Item</a> | <a href="../idiademimplicitchannel/">ImplicitChannel &lt;Data&gt;</a>.<a href="../../properties/idiademimplicitchannel-channelgroup/">ChannelGroup</a> | <a href="../idiademproperty/">Property &lt;Data&gt;</a>.<a href="../../properties/idiademproperty-element/">Element</a> | <a href="../idiademroot/">Root &lt;Data&gt;</a>.<a href="../../properties/idiademroot-activechannelgroup/">ActiveChannelGroup</a> | <a href="../idiademvideochannel/">VideoChannel &lt;Data&gt;</a>.<a href="../../properties/idiademvideochannel-channelgroup/">ChannelGroup</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademChannelGroup.HTM`*
