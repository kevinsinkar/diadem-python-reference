---
title: "IImplicitChannel.Properties"
description: "Contains the Properties collection associated with an implicit channel."
---

# IImplicitChannel.Properties

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Properties for ImplicitChannel

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Contains the Properties collection associated with an implicit channel.

## Signature

```python
return_value = obj.Properties
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyChn in Root.ChannelGroups(1).Channels:
    if oMyChn.IsKindOf(eImplicit):
        for oMyProp in oMyChn.Properties:
            if oMyProp.Name == "Sensor_Type":
                bFound = TRUE
        if not bFound:
            oMyChn.Properties.Add("Sensor_type","TC-N")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Properties_IImplicitChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
