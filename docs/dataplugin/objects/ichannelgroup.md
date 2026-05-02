---
title: "IChannelGroup"
description: "The ChannelGroup object provides a channel group including the associated channels and properties."
---

# IChannelGroup

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: ChannelGroup <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

The ChannelGroup object provides a channel group including the associated channels and properties.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.ChannelGroups.RemoveAll
oMyGrp.Properties.Add("Time",CreateTime(2004,6,12,10,0,0,0,0,0))
oMyGrp.Properties.Add("Tester","CK")
for i in range(1, 100 + 1):
    oMyChn.Values(i) = cdbl(i/100000)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ichannelgroup-channels/">Channels</a> | <a href="../../properties/ichannelgroup-name/">Name</a> | <a href="../../properties/ichannelgroup-properties/">Properties</a> | <a href="../../properties/ichannelgroup-root/">Root</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ichannel/">Channel &lt;DataPlugin&gt;</a>.<a href="../../properties/ichannel-channelgroup/">ChannelGroup</a> | <a href="../../collections/channelgroups/">ChannelGroups &lt;DataPlugin&gt;</a>.<a href="../../methods/ichannelgroups-add/">Add</a> | <a href="../../collections/channelgroups/">ChannelGroups &lt;DataPlugin&gt;</a>.<a href="../../methods/ichannelgroups-item/">Item</a> | <a href="../iimplicitchannel/">ImplicitChannel</a>.<a href="../../properties/iimplicitchannel-channelgroup/">ChannelGroup</a> | <a href="../iprocessedchannel/">ProcessedChannel</a>.<a href="../../properties/iprocessedchannel-channelgroup/">ChannelGroup</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Root Object Overview</a> | <a href="#" data-unresolved="1">Store Object Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IChannelGroup.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
