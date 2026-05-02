---
title: "IChannel.Properties"
description: "Contains the Properties collection associated with a Channel object."
---

# IChannel.Properties

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Properties for Channel <DataPlugin>

Contains the Properties collection associated with a Channel object.

## Signature

```python
return_value = obj.Properties
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyChn = Root.ChannelGroups(1).Channels(3)
for oMyProp in oMyChn.Properties:
    if oMyProp.Name == "Sensor_Type":
        bFound = TRUE
if not bFound:
    oMyChn.Properties.Add("Sensor_type","TC-N")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Properties_IChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
