---
title: "IUSISimplifiedStore.PluginName"
description: "Contains the name of the DataPlugin that opens the data store."
---

# IUSISimplifiedStore.PluginName

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: PluginName for Store

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Contains the name of the DataPlugin that opens the data store.

## Signature

```python
obj.PluginName
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.Properties.Add("PluginName",FromStore.PluginName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_PluginName_IUSISimplifiedStore.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
