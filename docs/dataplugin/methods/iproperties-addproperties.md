---
title: "IProperties.AddProperties"
description: "Adds a list of properties to the Properties collection."
---

# IProperties.AddProperties

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: AddProperties for Properties <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Adds a list of properties to the Properties collection.

## Signature

```python
obj.AddProperties(Properties, Prefix)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>If the specified custom property exists, the <span class="Monospace">AddProperties</span> method overwrites the value of the property.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.ChannelGroups(1).Properties.AddProperties(Root.ChannelGroups(2).Properties)
```

```python
for j in range(1, FromStore.Children.Count + 1):
    if FromStore.Children.Item(j).IsKindOf(eStoreChannelGroup):
        Root.Properties.AddProperties(StoreElement.Properties, StoreElement.Type + i + "_")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_AddProperties_IProperties.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
