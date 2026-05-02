---
title: "IProcessedChannel.Channels"
description: "Contains the ChannelsToProcess collection associated with a ProcessedChannel object."
---

# IProcessedChannel.Channels

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Channels for ProcessedChannel

Contains the ChannelsToProcess collection associated with a ProcessedChannel object.

## Signature

```python
return_value = obj.Channels
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for Channel in ChannelGroup.Channels:
    if Channel.IsKindOf(eDirectAccess) and (Channel.DataType == eR64):
        ProcessedChn.Channels.Add(Channel)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Channels_IProcessedChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
