---
title: "IChannelGroups.Count"
description: "Returns the number of elements in a ChannelGroups collection."
---

# IChannelGroups.Count

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Count for ChannelGroups <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Returns the number of elements in a ChannelGroups collection.

## Signature

```python
obj.Count
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for j in range(1, Root.Channelgroups.Count + 1):
    oMyProp = Root.ChannelGroups(j).Properties
    for i in range(1, oMyProp.Count + 1):
        if oMyProp(i).Name == "Test_Status":
            oMyProp(i).Value = "failed"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Count_IChannelGroups.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
