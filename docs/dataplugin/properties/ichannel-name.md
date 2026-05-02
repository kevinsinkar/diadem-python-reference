---
title: "IChannel.Name"
description: "Receives the name of a Channel object."
---

# IChannel.Name

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Name for Channel <DataPlugin>

Receives the name of a Channel object.

## Signature

```python
obj.Name
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, Root.ChannelGroups.Count + 1):
    for oMyChn in Root.ChannelGroups(i).Channels:
        if oMyChn.Name == "Temp":
            oMyChn.Properties.Add("Sensor_Type","TC-J")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Name_IChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
