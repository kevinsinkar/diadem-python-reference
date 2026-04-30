---
title: "IProcessedChannel.Size"
description: "Returns the current number of values in a channel."
---

# IProcessedChannel.Size

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Size for ProcessedChannel

Returns the current number of values in a channel.

## Signature

```python
obj.Size
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
ProcessedChn = ChannelGroup.Channels.AddProcessedChannel("MyChannel",eR64,eAddProcessor)
for Channel in ChannelGroup.Channels:
    if Channel.IsKindOf(eDirectAccess) and (Channel.DataType = eR64):
        ProcessedChn.Channels.Add(Channel)

for i in range(1, ProcessedChn.Size + 1):
    Sum = Sum + ProcessedChn.Values(i)
ProcessedChn.Properties.Add("Sum",Sum)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Size_IProcessedChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
