---
title: "IProcessedChannel.Values"
description: "Returns the single value of a Channel at a specific channel position."
---

# IProcessedChannel.Values

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Values for ProcessedChannel

Returns the single value of a Channel at a specific channel position.

## Signature

```python
obj.Values(iIndex)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The <a href="../iprocessedchannel-size/">Size</a> property contains the current number of values of a channel.</td></tr></table>
</div>

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

*Source: `DataPlugin/Properties/DataPlugin_property_Values_IProcessedChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
