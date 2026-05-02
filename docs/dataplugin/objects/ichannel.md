---
title: "IChannel"
description: "The Channel object provides the channel values and the associated properties."
---

# IChannel

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: Channel <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

The Channel object provides the channel values and the associated properties.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, 100 + 1):
    oMyChn.Values(i) = cdbl(i/100000)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ichannel-channelgroup/">ChannelGroup</a> | <a href="../../properties/ichannel-datatype/">DataType</a> | <a href="../../properties/ichannel-factor/">Factor</a> | <a href="../../properties/ichannel-name/">Name</a> | <a href="../../properties/ichannel-offset/">Offset</a> | <a href="../../properties/ichannel-properties/">Properties</a> | <a href="../../properties/ichannel-reservedsize/">ReservedSize</a> | <a href="../../properties/ichannel-size/">Size</a> | <a href="../../properties/ichannel-values/">Values</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ichannel-addcharacteristics/">AddCharacteristics</a> | <a href="../../methods/ichannel-addwaveformproperties/">AddWaveformProperties</a> | <a href="../../methods/ichannel-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/channels/">Channels &lt;DataPlugin&gt;</a>.<a href="../../methods/ichannels-add/">Add</a> | <a href="../../collections/channels/">Channels &lt;DataPlugin&gt;</a>.<a href="../../methods/ichannels-item/">Item</a> | <a href="../../collections/channelstoprocess/">ChannelsToProcess</a>.<a href="../../methods/ichannelstoprocess-add/">Add</a> | <a href="../../collections/channelstoprocess/">ChannelsToProcess</a>.<a href="../../methods/ichannelstoprocess-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Root Object Overview</a> | <a href="#" data-unresolved="1">Store Object Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
