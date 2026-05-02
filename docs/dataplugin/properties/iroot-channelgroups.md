---
title: "IRoot.ChannelGroups"
description: "Contains the ChannelGroups collection associated with a Root object."
---

# IRoot.ChannelGroups

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: ChannelGroups for Root <DataPlugin>

Contains the ChannelGroups collection associated with a Root object.

## Signature

```python
return_value = obj.ChannelGroups
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for j in range(1, Root.ChannelGroups.Count + 1):
    oMyProp = Root.ChannelGroups(j).Properties
    for i in range(1, oMyProp.Count + 1):
        if oMyProp(i).Name == "Test_Status":
            oMyProp(i).Value = "failed"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_ChannelGroups_IRoot.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
