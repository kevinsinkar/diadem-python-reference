---
title: "IProcessedChannel.Properties"
description: "Contains the Properties collection associated with a ProcessedChannel object."
---

# IProcessedChannel.Properties

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Properties for ProcessedChannel

Contains the Properties collection associated with a ProcessedChannel object.

## Signature

```python
return_value = obj.Properties
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for Channel in ChannelGroup.Channels:
    if Channel.IsKindOf(eDirectAccess) and (Channel.DataType = eR64):
        ProcessedChn.Channels.Add(Channel)

if not ProcessedChn.Properties.Exists("Sensor_type"):
    ProcessedChn.Properties.Add("Sensor_type","TC-N")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Properties_IProcessedChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
