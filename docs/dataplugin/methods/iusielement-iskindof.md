---
title: "IUSIElement.IsKindOf"
description: "Checks whether an Element object is a certain type."
---

# IUSIElement.IsKindOf

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: IsKindOf for Element <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Checks whether an Element object is a certain type.

## Signature

```python
iIsKindOf = Object.IsKindOf(Type)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for StoreElement in FromStore.Children:
    if StoreElement.IsKindOf(eStoreChannelGroup):
        TDMGroup = Root.ChannelGroups.Add(StoreElement.Name)
        TDMGroup.Properties.AddProperties(StoreElement.Properties)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_IsKindOf_IUSIElement.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
