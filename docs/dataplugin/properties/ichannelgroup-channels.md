---
title: "IChannelGroup.Channels"
description: "Contains the Channels collection associated with a ChannelGroup object."
---

# IChannelGroup.Channels

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Channels for ChannelGroup <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

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
