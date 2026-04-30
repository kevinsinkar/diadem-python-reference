---
title: "IProcessedChannel"
description: "The ProcessedChannel object provides a channel, which combines values from other channels ( ChannelsToProcess ), and the associated properties."
---

# IProcessedChannel

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: ProcessedChannel

The ProcessedChannel object provides a channel, which combines values from other channels ( ChannelsToProcess ), and the associated properties.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for Channel in Channelgroup.Channels:
    if Channel.IsKindOf(eDirectAccess) and (Channel.DataType = eR64):
        ProcessedChn.Channels.Add(Channel)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iprocessedchannel-channelgroup/">ChannelGroup</a> | <a href="../../properties/iprocessedchannel-channels/">Channels</a> | <a href="../../properties/iprocessedchannel-datatype/">DataType</a> | <a href="../../properties/iprocessedchannel-factor/">Factor</a> | <a href="../../properties/iprocessedchannel-name/">Name</a> | <a href="../../properties/iprocessedchannel-offset/">Offset</a> | <a href="../../properties/iprocessedchannel-properties/">Properties</a> | <a href="../../properties/iprocessedchannel-size/">Size</a> | <a href="../../properties/iprocessedchannel-values/">Values</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iprocessedchannel-addcharacteristics/">AddCharacteristics</a> | <a href="../../methods/iprocessedchannel-addwaveformproperties/">AddWaveformProperties</a> | <a href="../../methods/iprocessedchannel-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/channels/">Channels &lt;DataPlugin&gt;</a>.<a href="../../methods/ichannels-addprocessedchannel/">AddProcessedChannel</a> | <a href="../../collections/channels/">Channels &lt;DataPlugin&gt;</a>.<a href="../../methods/ichannels-item/">Item</a> | <a href="../../collections/channelstoprocess/">ChannelsToProcess</a>.<a href="../../methods/ichannelstoprocess-add/">Add</a> | <a href="../../collections/channelstoprocess/">ChannelsToProcess</a>.<a href="../../methods/ichannelstoprocess-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IProcessedChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
