---
title: "IProcessedChannel.ChannelGroup"
description: "Specifies the channel group to which the ProcessedChannel channel type is assigned."
---

# IProcessedChannel.ChannelGroup

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: ChannelGroup for ProcessedChannel

Specifies the channel group to which the ProcessedChannel channel type is assigned.

## Signature

```python
return_value = obj.ChannelGroup
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, Root.ChannelGroups.Count + 1):
    for oMyChn in Root.ChannelGroups(i).Channels:
        if oMyChn.Name = "Temp":
            MsgBoxDisp(oMyChn.ChannelGroup.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_ChannelGroup_IProcessedChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
