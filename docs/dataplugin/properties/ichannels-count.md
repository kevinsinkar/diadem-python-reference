---
title: "IChannels.Count"
description: "Returns the number of elements in a Channels collection."
---

# IChannels.Count

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Count for Channels <DataPlugin>

Returns the number of elements in a Channels collection.

## Signature

```python
obj.Count
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, Root.ChannelGroups(1).Channels.Count + 1):
    for oMyProp in Root.ChannelGroups(1).Channels(I).Properties:
        if oMyProp.Name == "Offset":
            oMyProp.Value = oMyProp.Value * 2
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Count_IChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
