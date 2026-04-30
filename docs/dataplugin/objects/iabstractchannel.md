---
title: "IAbstractChannel"
description: "The AbstractChannel object provides the channel values and the associated properties. The AbstractChannel object corresponds with a Channel , a DirectAccessChan"
---

# IAbstractChannel

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: AbstractChannel

The AbstractChannel object provides the channel values and the associated properties. The AbstractChannel object corresponds with a Channel , a DirectAccessChannel or an ImplicitChannel .

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyChn in Root.ChannelGroups(1).Channels:
    if (oMyChn.IsKindOf(eNormal)):
        oMyChn.Properties.Add("DataType", oMyChn.DataType)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iabstractchannel-datatype/">DataType</a> | <a href="../../properties/iabstractchannel-name/">Name</a> | <a href="../../properties/iabstractchannel-properties/">Properties</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iabstractchannel-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/channels/">Channels &lt;DataPlugin&gt;</a>.<a href="../../methods/ichannels-item/">Item</a> | <a href="../../collections/channelstoprocess/">ChannelsToProcess</a>.<a href="../../methods/ichannelstoprocess-add/">Add</a> | <a href="../../collections/channelstoprocess/">ChannelsToProcess</a>.<a href="../../methods/ichannelstoprocess-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IAbstractChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
