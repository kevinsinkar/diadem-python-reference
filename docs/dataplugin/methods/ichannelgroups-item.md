---
title: "IChannelGroups.Item"
description: "Returns the ChannelGroup object associated with a specific name or with a specific index."
---

# IChannelGroups.Item

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Item for ChannelGroups <DataPlugin>

Returns the ChannelGroup object associated with a specific name or with a specific index.

## Signature

```python
return_value = obj.Item(GrpNameOrIndex)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyChn in Root.ChannelGroups.Item(3).Channels:
    if oMyChn.Name = "Meas_Cal":
        oMyChn.Properties.Add("Faktor", 5)
        oMyChn.Properties.Add("Offset", 50)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Item_IChannelGroups.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
