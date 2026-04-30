---
title: "IChannelGroup.Channels"
description: "Contains the Channels collection associated with a ChannelGroup object."
---

# IChannelGroup.Channels

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Channels for ChannelGroup <DataPlugin>

Contains the Channels collection associated with a ChannelGroup object.

## Signature

```python
return_value = obj.Channels
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyChn in Root.ChannelGroups("QT_34-51_Lower").Channels:
    oMyChn.Properties.Add("Sensor_Type","TC-N")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Channels_IChannelGroup.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
