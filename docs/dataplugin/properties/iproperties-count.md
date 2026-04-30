---
title: "IProperties.Count"
description: "Returns the number of elements in a Properties collection."
---

# IProperties.Count

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Count for Properties <DataPlugin>

Returns the number of elements in a Properties collection.

## Signature

```python
obj.Count
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyProp = Root.ChannelGroups(1).Properties
for i in range(1, oMyProp.Count + 1):
    if oMyProp(i).Name = "Test_Status":
        oMyProp(i).Value = "failed"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Count_IProperties.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
