---
title: "IChannelGroup.Properties"
description: "Contains the Properties collection associated with a ChannelGroup object."
---

# IChannelGroup.Properties

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Properties for ChannelGroup <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Contains the Properties collection associated with a ChannelGroup object.

## Signature

```python
return_value = obj.Properties
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyGrp = Root.ChannelGroups(1)
for oMyProp in oMyGrp.Properties:
    if oMyProp.Name == "Test_Status":
        bfound = TRUE
if not bFound:
    oMyGrp.Properties.Add("Test_Status","Pass")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Properties_IChannelGroup.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
