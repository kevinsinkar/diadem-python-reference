---
title: "IUSIElements.Count"
description: "Returns the number of elements in a Elements collection."
---

# IUSIElements.Count

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Count for Elements <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Returns the number of elements in a Elements collection.

## Signature

```python
obj.Count
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for j in range(1, FromStore.Children.Count + 1):
    if StoreElement.IsKindOf(eStoreChannelGroup):
        Root.Properties.Add("Composite"& right("0"&j,2), FromStore.Children.Item(j).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<div class="SeeAlso">
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Count_IUSIElements.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
