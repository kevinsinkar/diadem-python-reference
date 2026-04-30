---
title: "IAbstractChannel.Name"
description: "Specifies a channel name."
---

# IAbstractChannel.Name

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Name for AbstractChannel

Specifies a channel name.

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
        if oMyChn.Name = "Temp":
            oMyChn.Properties.Add("Sensor_Type","TC-J")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Name_IAbstractChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
